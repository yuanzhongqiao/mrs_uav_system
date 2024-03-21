<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">多机器人系统集团无人机系统</font></font></h1><a id="user-content-multi-robot-systems-group-uav-system" class="anchor" aria-label="永久链接：多机器人系统集团无人机系统" href="#multi-robot-systems-group-uav-system"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/logos.png"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/logos.png" alt="标志" style="max-width: 100%;"></a></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/drone_collage.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/drone_collage.jpg" alt="缩略图" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"></font><a href="http://mrs.felk.cvut.cz" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">多机器人系统小组</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是</font></font><a href="https://www.cvut.cz/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">布拉格捷克技术大学</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">的一个机器人实验室</font><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">我们专注于多旋翼直升机，并专门为它们开发了这种控制、估计和仿真系统。</font><font style="vertical-align: inherit;">我们认为现实世界和可复制的实验应该支持机器人技术的出色研究和科学研究。</font><font style="vertical-align: inherit;">因此，我们的平台旨在允许对规划、控制、估计、计算机视觉、跟踪等方法进行安全的现实实验验证。</font></font></p>
<blockquote>
<p dir="auto"><g-emoji class="g-emoji" alias="warning"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">⚠️</font></font></g-emoji> <strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请注意：此自述文件需要修改。</font></font></strong></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">MRS无人机系统1.5正在发布，此页面需要更新。</font><font style="vertical-align: inherit;">请记住，此页面上的信息可能无效。</font><font style="vertical-align: inherit;">查看此</font></font><a href="https://docs.google.com/document/d/1NibHqNdyzzAYE7DNIMMq1HmzyFrBnISbzV17dP-waYw/edit?usp=sharing" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">WIP Google 文档</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">以了解最新消息和更改。</font></font></p>
</blockquote>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">TL;DR 与旧系统相比有何变化</font></font></h2><a id="user-content-tldr-what-has-changed-from-the-old-system" class="anchor" aria-label="永久链接：TL;DR 旧系统有何变化" href="#tldr-what-has-changed-from-the-old-system"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意：</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> MRS UAV 系统 v1.5 仍处于开发中，文档正在进行维护（</font></font><a href="https://github.com/ctu-mrs/mrs_uav_system/issues/169" data-hovercard-type="issue" data-hovercard-url="/ctu-mrs/mrs_uav_system/issues/169/hovercard"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Issue#169</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）。</font></font><a href="https://docs.google.com/document/d/1NibHqNdyzzAYE7DNIMMq1HmzyFrBnISbzV17dP-waYw/edit?usp=sharing" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以在此处WIP Google 文档</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">中找到更改和新说明</font><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">欢迎任何反馈（您可以使用此存储库中的问题或对 Google 文档发表评论）！</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">系统属性</font></font></h2><a id="user-content-system-properties" class="anchor" aria-label="永久链接：系统属性" href="#system-properties"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该系统是</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">建立在</font></font><a href="https://www.ros.org/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">机器人操作系统</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Noetic之上，</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">意味着完全在配套计算机上执行，</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可以控制欠驱动多旋翼直升机，</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">包含控制、状态估计、绘图和规划管道。</font></font></li>
</ul>
<p dir="auto"><animated-image data-catalyst=""><a target="_blank" rel="noopener noreferrer" href="https://github.com/ctu-mrs/mrs_uav_system/raw/gifs/gazebo_circle.gif" data-target="animated-image.originalLink"><img src="https://github.com/ctu-mrs/mrs_uav_system/raw/gifs/gazebo_circle.gif" alt="" style="max-width: 100%; display: inline-block;" data-target="animated-image.originalImage"></a>
      <span class="AnimatedImagePlayer" data-target="animated-image.player" hidden="">
        <a data-target="animated-image.replacedLink" class="AnimatedImagePlayer-images" href="https://github.com/ctu-mrs/mrs_uav_system/raw/gifs/gazebo_circle.gif" target="_blank">
          
        <span data-target="animated-image.imageContainer">
            <img data-target="animated-image.replacedImage" alt="gazebo_circle.gif" class="AnimatedImagePlayer-animatedImage" src="https://github.com/ctu-mrs/mrs_uav_system/raw/gifs/gazebo_circle.gif" style="display: block; opacity: 1;">
          <canvas class="AnimatedImagePlayer-stillImage" aria-hidden="true" width="813" height="200"></canvas></span></a>
        <button data-target="animated-image.imageButton" class="AnimatedImagePlayer-images" tabindex="-1" aria-label="Play gazebo_circle.gif" hidden=""></button>
        <span class="AnimatedImagePlayer-controls" data-target="animated-image.controls" hidden="">
          <button data-target="animated-image.playButton" class="AnimatedImagePlayer-button" aria-label="Play gazebo_circle.gif">
            <svg aria-hidden="true" focusable="false" class="octicon icon-play" width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M4 13.5427V2.45734C4 1.82607 4.69692 1.4435 5.2295 1.78241L13.9394 7.32507C14.4334 7.63943 14.4334 8.36057 13.9394 8.67493L5.2295 14.2176C4.69692 14.5565 4 14.1739 4 13.5427Z">
            </path></svg>
            <svg aria-hidden="true" focusable="false" class="octicon icon-pause" width="16" height="16" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg">
              <rect x="4" y="2" width="3" height="12" rx="1"></rect>
              <rect x="9" y="2" width="3" height="12" rx="1"></rect>
            </svg>
          </button>
          <a data-target="animated-image.openButton" aria-label="Open gazebo_circle.gif in new window" class="AnimatedImagePlayer-button" href="https://github.com/ctu-mrs/mrs_uav_system/raw/gifs/gazebo_circle.gif" target="_blank">
            <svg aria-hidden="true" class="octicon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" width="16" height="16">
              <path fill-rule="evenodd" d="M10.604 1h4.146a.25.25 0 01.25.25v4.146a.25.25 0 01-.427.177L13.03 4.03 9.28 7.78a.75.75 0 01-1.06-1.06l3.75-3.75-1.543-1.543A.25.25 0 0110.604 1zM3.75 2A1.75 1.75 0 002 3.75v8.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 12.25v-3.5a.75.75 0 00-1.5 0v3.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25v-8.5a.25.25 0 01.25-.25h3.5a.75.75 0 000-1.5h-3.5z"></path>
            </svg>
          </a>
        </span>
      </span></animated-image></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><a href="https://ctu-mrs.github.io/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">文档</font></font></a></h2><a id="user-content-documentation" class="anchor" aria-label="永久链接：文档" href="#documentation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">主要文档来源位于： https: </font></font><a href="https://ctu-mrs.github.io/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">//ctu-mrs.github.io/</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">然而，该网站只触及了其应包含内容的表面（我们知道这一点）。</font><font style="vertical-align: inherit;">我们的系统是一个以研究为导向的平台，并且发展迅速。</font><font style="vertical-align: inherit;">我们的大多数用户要么是研究人员（已经了解该平台），要么是新生（可能不了解 ROS）。</font><font style="vertical-align: inherit;">为这样的受众维护最新的文档是一项艰巨的工作，因为我们主要是在将系统用于我们的研究时开发该系统。</font><font style="vertical-align: inherit;">因此，我们的目标是教育学生查看软件包（每个软件包都包含自己的自述文件），探索启动文件，并能够阅读我们努力保持可读性的代码。</font></font></p>
<p dir="auto"><a href="https://github.com/ctu-mrs/mrs_uav_system/raw/diagram/mrs_uav_system_diagram.png"><img src="https://github.com/ctu-mrs/mrs_uav_system/raw/diagram/mrs_uav_system_diagram.png" alt="" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">控制和估计系统在文章</font></font><a href="https://doi.org/10.1007/s10846-021-01383-5" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">doi.org/10.1007/s10846-021-01383-5</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，</font></font><a href="https://link.springer.com/content/pdf/10.1007/s10846-021-01383-5.pdf" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">pdf</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">中描述：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>Baca, T., Petrlik, M., Vrba, M., Spurny, V., Penicka, R., Hert, D., and Saska, M.,
"The MRS UAV System: Pushing the Frontiers of Reproducible Research, Real-world Deployment, and
Education with Autonomous Unmanned Aerial Vehicles", J Intell Robot Syst 102, 26 (2021).
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="Baca, T., Petrlik, M., Vrba, M., Spurny, V., Penicka, R., Hert, D., and Saska, M.,
&quot;The MRS UAV System: Pushing the Frontiers of Reproducible Research, Real-world Deployment, and
Education with Autonomous Unmanned Aerial Vehicles&quot;, J Intell Robot Syst 102, 26 (2021)." tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装</font></font></h2><a id="user-content-installation" class="anchor" aria-label="永久链接：安装" href="#installation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">原生安装</font></font></h3><a id="user-content-native-installation" class="anchor" aria-label="永久链接：本机安装" href="#native-installation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装机器人操作系统（Noetic）：</font></font></li>
</ol>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>curl https://ctu-mrs.github.io/ppa-unstable/add_ros_ppa.sh <span class="pl-k">|</span> bash
sudo apt install ros-noetic-desktop-full</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="curl https://ctu-mrs.github.io/ppa-unstable/add_ros_ppa.sh | bash
sudo apt install ros-noetic-desktop-full" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ol start="2" dir="auto">
<li>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">根据</font></font><a href="http://wiki.ros.org/ROS/Tutorials/InstallingandConfiguringROSEnvironment" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">http://wiki.ros.org/ROS/Tutorials/InstallingandConfiguringROSEnvironment配置你的ROS环境</font></font></a></p>
</li>
<li>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">选择您要安装的 MRS 无人机系统版本。</font></font></p>
</li>
</ol>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对于</font></font><strong><a href="https://github.com/ctu-mrs/ppa-stable"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">稳定</font></font></a></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">版本，添加稳定的 PPA：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>curl https://ctu-mrs.github.io/ppa-stable/add_ppa.sh <span class="pl-k">|</span> bash</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="curl https://ctu-mrs.github.io/ppa-stable/add_ppa.sh | bash" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对于</font></font><strong><a href="https://github.com/ctu-mrs/ppa-unstable"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不稳定</font></font></a></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（每夜构建）的系统，添加不稳定的 PPA：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>curl https://ctu-mrs.github.io/ppa-unstable/add_ppa.sh <span class="pl-k">|</span> bash</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="curl https://ctu-mrs.github.io/ppa-unstable/add_ppa.sh | bash" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ol start="4" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装MRS无人机系统：</font></font></li>
</ol>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>sudo apt install ros-noetic-mrs-uav-system-full</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="sudo apt install ros-noetic-mrs-uav-system-full" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ol start="5" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">启动示例 Gazebo 模拟会话：</font></font></li>
</ol>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>roscd mrs_uav_gazebo_simulation/tmux/one_drone
./start.sh</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="roscd mrs_uav_gazebo_simulation/tmux/one_drone
./start.sh" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">奇点容器</font></font></h3><a id="user-content-singularity-containers" class="anchor" aria-label="永久链接：奇点容器" href="#singularity-containers"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请点击此链接了解如何使用 Singularity 运行我们的系统。</font></font></p>
<ul dir="auto">
<li><a href="https://github.com/ctu-mrs/mrs_singularity"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">夫人奇点</font></font></a></li>
</ul>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开始开发自己的包</font></font></h3><a id="user-content-start-developing-your-own-package" class="anchor" aria-label="永久链接：开始开发自己的包" href="#start-developing-your-own-package"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">本教程假设您已使用上述命令安装了 MRS 无人机系统。</font></font></p>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">设置catkin工作区：</font></font></li>
</ol>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>source /opt/ros/noetic/setup.bash             # source the general ROS workspace so that the local one will extend it and see all the packages
mkdir -p ~/workspace/src &amp;&amp; cd ~/workspace    # create the workspace folder in home and cd to it
catkin init -w ~/workspace                    # initialize the new workspace
# setup basic compilation profiles
catkin config --profile debug --cmake-args -DCMAKE_BUILD_TYPE=Debug -DCMAKE_EXPORT_COMPILE_COMMANDS=ON -DCMAKE_CXX_FLAGS='-std=c++17 -Og' -DCMAKE_C_FLAGS='-Og'
catkin config --profile release --cmake-args -DCMAKE_BUILD_TYPE=Release -DCMAKE_EXPORT_COMPILE_COMMANDS=ON -DCMAKE_CXX_FLAGS='-std=c++17'
catkin config --profile reldeb --cmake-args -DCMAKE_BUILD_TYPE=RelWithDebInfo -DCMAKE_EXPORT_COMPILE_COMMANDS=ON -DCMAKE_CXX_FLAGS='-std=c++17'
catkin profile set reldeb                     # set the reldeb profile as active
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="source /opt/ros/noetic/setup.bash             # source the general ROS workspace so that the local one will extend it and see all the packages
mkdir -p ~/workspace/src &amp;&amp; cd ~/workspace    # create the workspace folder in home and cd to it
catkin init -w ~/workspace                    # initialize the new workspace
# setup basic compilation profiles
catkin config --profile debug --cmake-args -DCMAKE_BUILD_TYPE=Debug -DCMAKE_EXPORT_COMPILE_COMMANDS=ON -DCMAKE_CXX_FLAGS='-std=c++17 -Og' -DCMAKE_C_FLAGS='-Og'
catkin config --profile release --cmake-args -DCMAKE_BUILD_TYPE=Release -DCMAKE_EXPORT_COMPILE_COMMANDS=ON -DCMAKE_CXX_FLAGS='-std=c++17'
catkin config --profile reldeb --cmake-args -DCMAKE_BUILD_TYPE=RelWithDebInfo -DCMAKE_EXPORT_COMPILE_COMMANDS=ON -DCMAKE_CXX_FLAGS='-std=c++17'
catkin profile set reldeb                     # set the reldeb profile as active" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ol start="2" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以重新利用我们的示例之一作为起点（可选）：</font></font></li>
</ol>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code># it is good practice to not clone ROS packages directly into a workspace, so let's use a separate directory for this
git clone git@github.com:ctu-mrs/mrs_core_examples.git ~/git/mrs_core_examples                    # clone this repository (recommended, requires private key on Github)
# git clone https://github.com/ctu-mrs/mrs_core_examples.git ~/git/mrs_core_examples              # if you do not have a private key set up on Github, you can use https instead of ssh
export NEW_PACKAGE=replaceme                                                                      # fill the NEW_NAME variable with your desired name of the new package (no spaces)
cp -r ~/git/mrs_core_examples/cpp/waypoint_flier ~/git/$NEW_PACKAGE                               # copy an example package (e.g. the waypoint_flier)
cp ~/git/mrs_core_examples/repurpose_package.sh ~/git/$NEW_PACKAGE                                # copy the repurpose_package.sh script to the new package
cd ~/git/$NEW_PACKAGE &amp;&amp; ./repurpose_package.sh example_waypoint_flier $NEW_PACKAGE --camel-case  # use the script to replace all occurences of the old name
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# it is good practice to not clone ROS packages directly into a workspace, so let's use a separate directory for this
git clone git@github.com:ctu-mrs/mrs_core_examples.git ~/git/mrs_core_examples                    # clone this repository (recommended, requires private key on Github)
# git clone https://github.com/ctu-mrs/mrs_core_examples.git ~/git/mrs_core_examples              # if you do not have a private key set up on Github, you can use https instead of ssh
export NEW_PACKAGE=replaceme                                                                      # fill the NEW_NAME variable with your desired name of the new package (no spaces)
cp -r ~/git/mrs_core_examples/cpp/waypoint_flier ~/git/$NEW_PACKAGE                               # copy an example package (e.g. the waypoint_flier)
cp ~/git/mrs_core_examples/repurpose_package.sh ~/git/$NEW_PACKAGE                                # copy the repurpose_package.sh script to the new package
cd ~/git/$NEW_PACKAGE &amp;&amp; ./repurpose_package.sh example_waypoint_flier $NEW_PACKAGE --camel-case  # use the script to replace all occurences of the old name" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ol start="3" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">将您的包链接到工作区并构建它（下面的代码假设您设置了变量</font></font><code>NEW_PACKAGE</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）：</font></font></li>
</ol>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>ln -s ~/git/$NEW_PACKAGE ~/workspace/src         # create a symbolic link of the package to the workspace
cd ~/workspace/src &amp;&amp; catkin build $NEW_PACKAGE  # build the package within the workspace
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="ln -s ~/git/$NEW_PACKAGE ~/workspace/src         # create a symbolic link of the package to the workspace
cd ~/workspace/src &amp;&amp; catkin build $NEW_PACKAGE  # build the package within the workspace" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ol start="4" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">现在，您可以使用新包：</font></font></li>
</ol>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>source ~/workspace/devel/setup.bash     # source the workspace to see the packages within (if you don't use bash, source the appropriate script instead)
roscd $NEW_PACKAGE                      # now ROS knows about your new package and you can roscd to it
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="source ~/workspace/devel/setup.bash     # source the workspace to see the packages within (if you don't use bash, source the appropriate script instead)
roscd $NEW_PACKAGE                      # now ROS knows about your new package and you can roscd to it" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意：</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">建议将</font></font><code>source ~/workspace/devel/setup.bash</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">命令添加到您的命令中</font></font><code>~/.bashrc</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，以便在每个新工作区中自动执行。</font></font></p>
<ol start="5" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为您的新包创建一个远程包（取决于您的 git 服务器）并推送到它：</font></font></li>
</ol>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>cd ~/workspace/src/$NEW_PACKAGE &amp;&amp; git add . &amp;&amp; git commit -m "initial commit"  # create the first commit in the new repository
git remote add origin &lt;your-new-remote&gt;                                         # replace &lt;your-new-remote&gt;
git push --set-upstream origin master                                           # push your initial commit
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="cd ~/workspace/src/$NEW_PACKAGE &amp;&amp; git add . &amp;&amp; git commit -m &quot;initial commit&quot;  # create the first commit in the new repository
git remote add origin <your-new-remote>                                         # replace <your-new-remote>
git push --set-upstream origin master                                           # push your initial commit" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意：</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在开发过程中不要忘记</font></font><code>git commit</code> <code>git push</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">定期！</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">系统组成</font></font></h2><a id="user-content-system-components" class="anchor" aria-label="永久链接：系统组件" href="#system-components"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">主要元包</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">内容</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">存储库</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">包裹</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">MRS无人机系统</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">无人机核心及无人机模块</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_uav_system"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_uav_system</font></font></a></td>
<td><code>ros-noetic-mrs-uav-system</code></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">MRS 无人机系统 - 完整版</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">全部如下</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_uav_system"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_uav_system</font></font></a></td>
<td><code>ros-noetic-mrs-uav-system-full</code></td>
</tr>
</tbody>
</table>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">元包</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">存储库</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">包裹</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">无人机核心</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_uav_core"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_uav_core</font></font></a></td>
<td><code>ros-noetic-mrs-uav-core</code></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">无人机模块</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_uav_modules"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_uav_模块</font></font></a></td>
<td><code>ros-noetic-mrs-uav-modules</code></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Octomap 测绘+规划</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_octomap_mapping_planning"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_octomap_mapping_planning</font></font></a></td>
<td><code>ros-noetic-mrs-octomap-mapping-planning</code></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ALOAM核心</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_aloam_core"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_aloam_core</font></font></a></td>
<td><code>ros-noetic-mrs-aloam-core</code></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LIO-SAM核心</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_liosam_core"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_liosam_core</font></font></a></td>
<td><code>ros-noetic-mrs-liosam-core</code></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">赫克托·科尔</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_hector_core"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_hector_core</font></font></a></td>
<td><code>ros-noetic-mrs-hector-core</code></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">OpenVINS 核心</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_open_vins_core"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_open_vins_core</font></font></a></td>
<td><code>ros-noetic-mrs-open-vins-core</code></td>
</tr>
</tbody>
</table>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模拟器</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">存储库</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">包裹</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">凉亭模拟</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_uav_gazebo_simulation"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_uav_gazebo_simulation</font></font></a></td>
<td><code>ros-noetic-mrs-uav-gazebo-simulation</code></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">MRS模拟</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_multirotor_simulator"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_多旋翼_模拟器</font></font></a></td>
<td><code>ros-noetic-mrs-multirotor-simulator</code></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">葛蓓亚模拟</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_uav_coppelia_simulation"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_uav_coppelia_simulation</font></font></a></td>
<td><code>ros-noetic-mrs-uav-coppelia-simulation</code></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">虚幻模拟</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_uav_unreal_simulation"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_uav_unreal_simulation</font></font></a></td>
<td><code>ros-noetic-mrs-uav-unreal-simulation</code></td>
</tr>
</tbody>
</table>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">硬件API插件</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">存储库</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">包裹</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">PX4 API</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_uav_px4_api"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_uav_px4_api</font></font></a></td>
<td><code>ros-noetic-mrs-uav-px4-api</code></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">大疆特洛API</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_uav_dji_tello_api"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_uav_dji_tello_api</font></font></a></td>
<td><code>ros-noetic-mrs-uav-dji-tello-api</code></td>
</tr>
</tbody>
</table>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">示例包</font></font></h2><a id="user-content-example-packages" class="anchor" aria-label="永久链接：示例包" href="#example-packages"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">例子</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">存储库</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">构建状态</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">核心示例</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_core_examples"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_core_examples</font></font></a></td>
<td><a href="https://github.com/ctu-mrs/mrs_core_examples/actions/workflows/ros_build_test.yml"><img src="https://github.com/ctu-mrs/mrs_core_examples/actions/workflows/ros_build_test.yml/badge.svg" alt="ros_build_测试" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">计算机视觉示例</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_computer_vision_examples"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_computer_vision_examples</font></font></a></td>
<td><a href="https://github.com/ctu-mrs/mrs_computer_vision_examples/actions/workflows/ros_build_test.yml"><img src="https://github.com/ctu-mrs/mrs_computer_vision_examples/actions/workflows/ros_build_test.yml/badge.svg" alt="ros_build_测试" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Gazebo 定制无人机示例</font></font></td>
<td><a href="https://github.com/ctu-mrs/mrs_gazebo_custom_drone_example"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_gazebo_custom_drone_example</font></font></a></td>
<td><a href="https://github.com/ctu-mrs/mrs_gazebo_custom_drone_example/actions/workflows/ros_build_test.yml"><img src="https://github.com/ctu-mrs/mrs_gazebo_custom_drone_example/actions/workflows/ros_build_test.yml/badge.svg" alt="ros_build_测试" style="max-width: 100%;"></a></td>
</tr>
</tbody>
</table>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">构建状态（</font></font><a href="https://github.com/ctu-mrs/buildfarm"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Buildfarm</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></h2><a id="user-content-build-status-buildfarm" class="anchor" aria-label="永久链接：构建状态（Buildfarm）" href="#build-status-buildfarm"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们利用验收测试来确定系统的可发布性并自动发布系统。</font><em><font style="vertical-align: inherit;">无论下面的测试和危险信号</font></em><font style="vertical-align: inherit;">的状态如何，我们系统的</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">稳定</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">版本都应该可以安装并始终工作</font><font style="vertical-align: inherit;">。</font></font><em><font style="vertical-align: inherit;"></font></em><font style="vertical-align: inherit;"></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">购电协议</font></font></h3><a id="user-content-ppas" class="anchor" aria-label="永久链接：购电协议" href="#ppas"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<table>
<thead>
<tr>
<th><a href="https://github.com/ctu-mrs/ppa-stable"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">稳定的</font></font></a></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">测试</font></font></th>
<th><a href="https://github.com/ctu-mrs/ppa-unstable"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不稳定</font></font></a></th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/ctu-mrs/ppa-stable/actions/workflows/deploy.yml"><img src="https://github.com/ctu-mrs/ppa-stable/actions/workflows/deploy.yml/badge.svg" alt="稳定的 ppa 构建" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/ppa-testing/actions/workflows/deploy.yml"><img src="https://github.com/ctu-mrs/ppa-testing/actions/workflows/deploy.yml/badge.svg" alt="测试-ppa-构建" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/ppa-unstable/actions/workflows/deploy.yml"><img src="https://github.com/ctu-mrs/ppa-unstable/actions/workflows/deploy.yml/badge.svg" alt="不稳定的 ppa 构建" style="max-width: 100%;"></a></td>
</tr>
</tbody>
</table>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">测试</font></font></h3><a id="user-content-testing" class="anchor" aria-label="永久链接：测试" href="#testing"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">相对。</font><font style="vertical-align: inherit;">候选人</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不稳定</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">测试覆盖率</font></font></th>
<th></th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/rostest_and_release_mrs_amd64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/rostest_and_release_mrs_amd64.yml/badge.svg" alt="rostest 和发布 mrs-amd64" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/rostest_unstable.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/rostest_unstable.yml/badge.svg" alt="rostest_不稳定" style="max-width: 100%;"></a></td>
<td><a href="https://ctu-mrs.github.io/buildfarm" rel="nofollow"><img src="https://camo.githubusercontent.com/dec4aef87bac8535e84cbb42ed4fafec85d07cf4ad55cde79994d58ccf57f9f9/68747470733a2f2f6374752d6d72732e6769746875622e696f2f6275696c646661726d2f62616467652e737667" alt="测试-ppa-构建" data-canonical-src="https://ctu-mrs.github.io/buildfarm/badge.svg" style="max-width: 100%;"></a></td>
<td></td>
</tr>
</tbody>
</table>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">x86-64/AMD64</font></font></h3><a id="user-content-x86-64amd64" class="anchor" aria-label="永久链接：x86-64/AMD64" href="#x86-64amd64"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<table>
<thead>
<tr>
<th></th>
<th><a href="https://github.com/ctu-mrs/ppa-stable"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">稳定的</font></font></a></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">发布候选</font></font></th>
<th><a href="https://github.com/ctu-mrs/ppa-unstable"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不稳定</font></font></a></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">MRS ROS 套餐</font></font></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_mrs_amd64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_mrs_amd64.yml/badge.svg" alt="稳定-mrs-amd64" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/rostest_and_release_mrs_amd64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/rostest_and_release_mrs_amd64.yml/badge.svg" alt="rostest 和发布 mrs-amd64" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_mrs_amd64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_mrs_amd64.yml/badge.svg" alt="不稳定-mrs-amd64" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">第三方 ROS 包</font></font></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_thirdparty_amd64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_thirdparty_amd64.yml/badge.svg" alt="稳定的第三方 amd64" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/testing_thirdparty_amd64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/testing_thirdparty_amd64.yml/badge.svg" alt="测试--第三方-amd64" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_thirdparty_amd64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_thirdparty_amd64.yml/badge.svg" alt="不稳定的第三方 amd64" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">非 ROS 包</font></font></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_nonbloom_amd64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_nonbloom_amd64.yml/badge.svg" alt="稳定非bloom-amd64" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/testing_nonbloom_amd64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/testing_nonbloom_amd64.yml/badge.svg" alt="测试--nonbloom-amd64" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_nonbloom_amd64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_nonbloom_amd64.yml/badge.svg" alt="不稳定-nonbloom-amd64" style="max-width: 100%;"></a></td>
</tr>
</tbody>
</table>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">AARCH64/ARM64</font></font></h3><a id="user-content-aarch64arm64" class="anchor" aria-label="永久链接：AARCH64/ARM64" href="#aarch64arm64"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<table>
<thead>
<tr>
<th></th>
<th><a href="https://github.com/ctu-mrs/ppa-stable"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">稳定的</font></font></a></th>
<th><a href="https://github.com/ctu-mrs/ppa-unstable"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不稳定</font></font></a></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">MRS ROS 套餐</font></font></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_mrs_arm64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_mrs_arm64.yml/badge.svg" alt="稳定-mrs-arm64" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_mrs_arm64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_mrs_arm64.yml/badge.svg" alt="不稳定-mrs-arm64" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">第三方 ROS 包</font></font></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_thirdparty_arm64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_thirdparty_arm64.yml/badge.svg" alt="稳定的第三方arm64" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_thirdparty_arm64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_thirdparty_arm64.yml/badge.svg" alt="不稳定的第三方arm64" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">非 ROS 包</font></font></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_nonbloom_arm64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/stable_nonbloom_arm64.yml/badge.svg" alt="稳定非布卢姆arm64" style="max-width: 100%;"></a></td>
<td><a href="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_nonbloom_arm64.yml"><img src="https://github.com/ctu-mrs/buildfarm/actions/workflows/unstable_nonbloom_arm64.yml/badge.svg" alt="不稳定非布卢姆arm64" style="max-width: 100%;"></a></td>
</tr>
</tbody>
</table>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">无人机</font></font></h2><a id="user-content-unmanned-aerial-vehicles" class="anchor" aria-label="永久链接：无人机" href="#unmanned-aerial-vehicles"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">MRS 无人机系统已针对 MRS 运营的以下无人机平台进行了预先配置。</font></font><a href="https://dronebuilder.fly4future.com/#/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">无人机平台可以从我们的合作伙伴公司Fly4Future</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">购买</font><font style="vertical-align: inherit;">。</font></font></p>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模拟</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">真正的无人机</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">大疆 f330</font></font></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/f330_simulation.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/f330_simulation.jpg" alt="" style="max-width: 100%;"></a></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/f330_real.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/f330_real.jpg" alt="" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">大疆 f450</font></font></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/f450_simulation.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/f450_simulation.jpg" alt="" style="max-width: 100%;"></a></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/f450_real.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/f450_real.jpg" alt="" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">霍利布罗 x500</font></font></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/x500_simulation.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/x500_simulation.jpg" alt="" style="max-width: 100%;"></a></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/x500_real.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/x500_real.jpg" alt="" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">大疆f550</font></font></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/f550_simulation.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/f550_simulation.jpg" alt="" style="max-width: 100%;"></a></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/f550_real.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/f550_real.jpg" alt="" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">塔罗牌t650</font></font></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/t650_simulation.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/t650_simulation.jpg" alt="" style="max-width: 100%;"></a></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/t650_real.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/t650_real.jpg" alt="" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">遥控无人机 m690</font></font></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/m690_simulation.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/m690_simulation.jpg" alt="" style="max-width: 100%;"></a></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/m690_real.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/m690_real.jpg" alt="" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">纳基二号</font></font></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/naki_simulation.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/naki_simulation.jpg" alt="" style="max-width: 100%;"></a></td>
<td><a target="_blank" rel="noopener noreferrer" href="/ctu-mrs/mrs_uav_system/blob/master/.fig/naki_real.jpg"><img src="/ctu-mrs/mrs_uav_system/raw/master/.fig/naki_real.jpg" alt="" style="max-width: 100%;"></a></td>
</tr>
</tbody>
</table>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">向后兼容性和更新</font></font></h2><a id="user-content-backwards-compatibility-and-updates" class="anchor" aria-label="永久链接：向后兼容性和更新" href="#backwards-compatibility-and-updates"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们不保证随时向后兼容。</font><font style="vertical-align: inherit;">该平台正在根据 MRS 集团的需求不断发展。</font><font style="vertical-align: inherit;">可以进行与用户的本地配置、模拟世界、tmux 会话等不兼容的更新。但是，当我们更改需要用户操作来保持兼容性的内容时，我们将在此存储库中创建一个标记为</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">users-read-的问题</font><font style="vertical-align: inherit;">我</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">单击此页面右上角的</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">“观看”</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">按钮订阅此存储库更新和问题。</font><font style="vertical-align: inherit;">需要用户操作的最新更改：</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">现在：</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">正在进行中的</font></font></strong> <strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">MRS 无人机系统 1.5：</font></font></strong> <a href="https://docs.google.com/document/d/1NibHqNdyzzAYE7DNIMMq1HmzyFrBnISbzV17dP-waYw/edit?usp=sharing" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">许多变化</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2023 年 1 月 17 日：</font></font><a href="https://github.com/ctu-mrs/mrs_uav_system/issues/150" data-hovercard-type="issue" data-hovercard-url="/ctu-mrs/mrs_uav_system/issues/150/hovercard"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">px4 固件 v1.13.2 更新</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2022 年 3 月 8 日：</font></font><a href="https://github.com/ctu-mrs/mrs_uav_system/issues/136" data-hovercard-type="issue" data-hovercard-url="/ctu-mrs/mrs_uav_system/issues/136/hovercard"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mrs_lib::Transformer 接口更新</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2021 年 12 月 9 日：</font></font><a href="https://github.com/ctu-mrs/mrs_uav_system/issues/126" data-hovercard-type="issue" data-hovercard-url="/ctu-mrs/mrs_uav_system/issues/126/hovercard"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不再使用 --march=native 进行构建</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2020 年 12 月 25 日：</font></font><a href="https://github.com/ctu-mrs/mrs_uav_system/issues/33" data-hovercard-type="issue" data-hovercard-url="/ctu-mrs/mrs_uav_system/issues/33/hovercard"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">更新了控制器界面，更新了推力曲线参数化</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2020年12月15日：</font></font><a href="https://github.com/ctu-mrs/mrs_uav_system/issues/32" data-hovercard-type="issue" data-hovercard-url="/ctu-mrs/mrs_uav_system/issues/32/hovercard"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模拟无人机产卵机制重做，Noetic更新</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2020 年 11 月 12 日：</font></font><a href="https://github.com/ctu-mrs/mrs_uav_system/issues/22" data-hovercard-type="issue" data-hovercard-url="/ctu-mrs/mrs_uav_system/issues/22/hovercard"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Gazebo 世界中的 GPS 坐标需要更改</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2020 年 11 月 12 日：</font></font><a href="https://github.com/ctu-mrs/mrs_uav_system/issues/21" data-hovercard-type="issue" data-hovercard-url="/ctu-mrs/mrs_uav_system/issues/21/hovercard"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">需要在模拟会话中启用测&ZeroWidthSpace;&ZeroWidthSpace;距仪融合</font></font></a></li>
</ul>
<div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">免责声明</font></font></h1><a id="user-content-disclaimer" class="anchor" aria-label="永久链接：免责声明" href="#disclaimer"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">本软件由版权所有者和贡献者“按原样”提供，不承担任何明示或默示的保证，包括但不限于适销性和特定用途适用性的默示保证。</font><font style="vertical-align: inherit;">在任何情况下，版权持有者或贡献者均不对任何直接、间接、附带、特殊、惩戒性或后果性损害（包括但不限于采购替代商品或服务；使用、数据或利润损失；或其他损失）承担责任。或业务中断），无论是何种原因造成的，并且基于任何责任理论，无论是合同责任、严格责任还是侵权行为（包括疏忽或其他），均因使用本软件而产生，即使已被告知可能发生此类损害。</font></font></p>
</article></div>
