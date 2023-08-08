<p align="center">
  <a href="#build-framework">
   <img src="https://raw.githubusercontent.com/armbian/build/master/.github/armbian-logo.png" alt="Armbian logo" width="144">
  </a><br>
  <strong>Armbian OS</strong><br>
<br>
<a href=https://github.com/armbian/os/actions/workflows/complete-artifact-matrix-all.yml><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/armbian/os/complete-artifact-matrix-all.yml?logo=githubactions&label=Artifacts%20make&style=for-the-badge&branch=main"></a>
<a href=https://github.com/armbian/os/actions/workflows/repository-update.yml><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/armbian/os/repository-update.yml?logo=githubactions&label=Repository%20update&style=for-the-badge&branch=main"></a>
<a href=https://github.com/armbian/os#latest-smoke-tests-results><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/armbian/os/smoke-tests.yml?logo=githubactions&label=Smoke%20tests&style=for-the-badge&branch=main"></a>
</p>


# What does this project do?

- Keeps build framework [packages artifacts](https://github.com/orgs/armbian/packages) cache up to date
- Keeps stable [apt.armbian.com](https://apt.armbian.com) and nightly [beta.armbian.com](https://beta.armbian.com) packages repository up to date
- Builds [nightly](https://github.com/armbian/os/releases) and [stable images](https://www.armbian.com/download/) and uploads them to Armbian CDN
- Keep synchronizing the selection of [3rd party](external) applications with Armbian repositories
- Tests install of all packages added onto stable and testing Debian and Ubuntu releases

# How to enable images?

If you want to enable build configurations, edit [yaml config files](/armbian/os/tree/main/userpatches) and send a pull request. ([example](https://github.com/armbian/os/commit/70f3be4f3d96e9a301be751d3ecf3a24394356f9) )

# When is this happening?

- Artifacts cache is updated every eight hours, starting at 0:00 AM UTC
- Repository update is updated once per day, at 3:00 AM UTC
- Smoke tests is executed after **repository update** is finished.
- Nightly images are build once per day, at 5:00 AM UTC
- Manually, when Armbian [release manager](https://github.com/orgs/armbian/teams/release-manager) executes a build action

# Latest smoke tests results:

- installs kernels, dtb and headers that are defined and supported by the board
- runs network and computing performance tests (7z benchmark)
- store armbianmonitor logs

<!--START_SECTION:data-section-->
<table width="100%"><tr><td align="left"><a href="https://paste.armbian.com/iniromezex">Orange Pi Win</a></td><td align="left">2023-08-08&nbsp;06:46:18</td><td align=right>legacy</td><td align=right>5.15.124-sunxi64</td><td align=right>669</td><td align=right>2656</td></tr><tr><td align="left"><a href="https://paste.armbian.com/xofaborufu">Orange Pi Win</a></td><td align="left">2023-08-08&nbsp;06:59:56</td><td align=right>current</td><td align=right>6.1.43-sunxi64</td><td align=right>770</td><td align=right>2874</td></tr><tr><td align="left"><a href="https://paste.armbian.com/locuvabexa">Orange Pi Win</a></td><td align="left">2023-08-08&nbsp;07:13:07</td><td align=right>edge</td><td align=right>6.4.8-sunxi64</td><td align=right>821</td><td align=right>2935</td></tr><tr><td align="left"><a href="https://paste.armbian.com/joxuxecazu">Tinker Board</a></td><td align="left">2023-08-08&nbsp;06:41:05</td><td align=right>current</td><td align=right>6.1.43-rockchip</td><td align=right>90</td><td align=right>5121</td></tr><tr><td align="left"><a href="https://paste.armbian.com/izahavuxax">Tinker Board</a></td><td align="left">2023-08-08&nbsp;06:47:53</td><td align=right>edge</td><td align=right>6.4.8-rockchip</td><td align=right>90</td><td align=right>4809</td></tr><tr><td align="left"><a href="https://paste.armbian.com/icurisagip">Espressobin</a></td><td align="left">2023-08-08&nbsp;06:52:31</td><td align=right>current</td><td align=right>5.15.124-mvebu64</td><td align=right>818</td><td align=right>1101</td></tr><tr><td align="left"><a href="https://paste.armbian.com/zokorepohi">Espressobin</a></td><td align="left">2023-08-08&nbsp;07:07:15</td><td align=right>edge</td><td align=right>6.1.43-mvebu64</td><td align=right>825</td><td align=right>1096</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ebuhosorij">Pine H64</a></td><td align="left">2023-08-08&nbsp;06:41:52</td><td align=right>current</td><td align=right>6.1.43-sunxi64</td><td align=right>840</td><td align=right>4116</td></tr><tr><td align="left"><a href="https://paste.armbian.com/sujaxesava">Pine H64</a></td><td align="left">2023-08-08&nbsp;06:48:53</td><td align=right>edge</td><td align=right>6.4.8-sunxi64</td><td align=right>853</td><td align=right>3990</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">UEFI x86</a></td><td align="left">2023-08-08&nbsp;06:48:41</td><td align=right>legacy</td><td align=right>5.15.124-x86</td><td align=right>786</td><td align=right>4780</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">UEFI x86</a></td><td align="left">2023-08-08&nbsp;06:55:21</td><td align=right>current</td><td align=right>6.1.43-x86</td><td align=right>748</td><td align=right>4769</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">UEFI x86</a></td><td align="left">2023-08-08&nbsp;07:02:29</td><td align=right>edge</td><td align=right>6.4.8-x86</td><td align=right>660</td><td align=right>4804</td></tr><tr><td align="left"><a href="n/a">RockPro 64</a></td><td align="left">2023-08-08&nbsp;06:33:42</td><td align=right>legacy</td><td align=right>n/a</td><td align=right>n/a</td><td align=right>n/a</td></tr><tr><td align="left"><a href="n/a">RockPro 64</a></td><td align="left">2023-08-08&nbsp;06:33:43</td><td align=right>current</td><td align=right>n/a</td><td align=right>n/a</td><td align=right>n/a</td></tr><tr><td align="left"><a href="n/a">RockPro 64</a></td><td align="left">2023-08-08&nbsp;06:33:45</td><td align=right>edge</td><td align=right>n/a</td><td align=right>n/a</td><td align=right>n/a</td></tr><tr><td align="left"><a href="https://paste.armbian.com/weciranuvi">Rockpi E</a></td><td align="left">2023-08-08&nbsp;06:45:57</td><td align=right>current</td><td align=right>6.1.43-rockchip64</td><td align=right>93</td><td align=right>3367</td></tr><tr><td align="left"><a href="https://paste.armbian.com/gexayahoto">Rockpi E</a></td><td align="left">2023-08-08&nbsp;06:59:17</td><td align=right>edge</td><td align=right>6.4.8-rockchip64</td><td align=right>90</td><td align=right>3346</td></tr><tr><td align="left"><a href="https://paste.armbian.com/irebujacib">Odroid C2</a></td><td align="left">2023-08-08&nbsp;06:44:28</td><td align=right>current</td><td align=right>6.1.43-meson64</td><td align=right>850</td><td align=right>3908</td></tr><tr><td align="left"><a href="https://paste.armbian.com/iboyuneluf">Odroid C2</a></td><td align="left">2023-08-08&nbsp;06:52:30</td><td align=right>edge</td><td align=right>6.4.8-meson64</td><td align=right>0</td><td align=right>4003</td></tr><tr><td align="left"><a href="https://paste.armbian.com/uwusibaper">NanoPi R6S</a></td><td align="left">2023-08-08&nbsp;06:36:15</td><td align=right>legacy</td><td align=right>5.10.160-rk35xx</td><td align=right>2440</td><td align=right>15610</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ajiveyogad">Orange Pi 3 LTS</a></td><td align="left">2023-08-08&nbsp;06:42:10</td><td align=right>current</td><td align=right>6.1.43-sunxi64</td><td align=right>910</td><td align=right>4044</td></tr><tr><td align="left"><a href="https://paste.armbian.com/imumanexos">Orange Pi 3 LTS</a></td><td align="left">2023-08-08&nbsp;06:51:48</td><td align=right>edge</td><td align=right>6.4.8-sunxi64</td><td align=right>830</td><td align=right>3915</td></tr><tr><td align="left"><a href="https://paste.armbian.com/evuxemonem">Odroid C4</a></td><td align="left">2023-08-08&nbsp;06:40:40</td><td align=right>current</td><td align=right>6.1.43-meson64</td><td align=right>820</td><td align=right>5646</td></tr><tr><td align="left"><a href="https://paste.armbian.com/pikekusetu">Odroid C4</a></td><td align="left">2023-08-08&nbsp;06:46:51</td><td align=right>edge</td><td align=right>6.4.8-meson64</td><td align=right>810</td><td align=right>5670</td></tr><tr><td align="left"><a href="https://paste.armbian.com/dujukutude">Rockpi 4B</a></td><td align="left">2023-08-08&nbsp;06:40:02</td><td align=right>current</td><td align=right>6.1.43-rockchip64</td><td align=right>730</td><td align=right>6496</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ehavugefuy">Rockpi 4B</a></td><td align="left">2023-08-08&nbsp;06:46:58</td><td align=right>edge</td><td align=right>6.4.8-rockchip64</td><td align=right>840</td><td align=right>6370</td></tr><tr><td align="left"><a href="https://paste.armbian.com/vidoxidupu">Banana Pi Pro</a></td><td align="left">2023-08-08&nbsp;06:46:46</td><td align=right>legacy</td><td align=right>5.15.124-sunxi</td><td align=right>364</td><td align=right>1029</td></tr><tr><td align="left"><a href="https://paste.armbian.com/urikeyozoz">Banana Pi Pro</a></td><td align="left">2023-08-08&nbsp;07:00:24</td><td align=right>current</td><td align=right>6.1.43-sunxi</td><td align=right>496</td><td align=right>1016</td></tr><tr><td align="left"><a href="https://paste.armbian.com/izutenowuq">Banana Pi Pro</a></td><td align="left">2023-08-08&nbsp;07:14:26</td><td align=right>edge</td><td align=right>6.4.8-sunxi</td><td align=right>409</td><td align=right>1017</td></tr><tr><td align="left"><a href="https://paste.armbian.com/umodonokic">ZeroPi</a></td><td align="left">2023-08-08&nbsp;06:47:07</td><td align=right>legacy</td><td align=right>5.15.124-sunxi</td><td align=right>543</td><td align=right>2655</td></tr><tr><td align="left"><a href="https://paste.armbian.com/hirugecewi">ZeroPi</a></td><td align="left">2023-08-08&nbsp;06:56:55</td><td align=right>current</td><td align=right>6.1.43-sunxi</td><td align=right>595</td><td align=right>2664</td></tr><tr><td align="left"><a href="https://paste.armbian.com/iwokujagux">ZeroPi</a></td><td align="left">2023-08-08&nbsp;07:07:03</td><td align=right>edge</td><td align=right>6.4.8-sunxi</td><td align=right>563</td><td align=right>2647</td></tr><tr><td align="left"><a href="https://paste.armbian.com/yikomokume">Cubietruck</a></td><td align="left">2023-08-08&nbsp;07:01:17</td><td align=right>legacy</td><td align=right>5.15.124-sunxi</td><td align=right>350</td><td align=right>1020</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ocejowitat">Cubietruck</a></td><td align="left">2023-08-08&nbsp;07:16:13</td><td align=right>current</td><td align=right>6.1.43-sunxi</td><td align=right>351</td><td align=right>1005</td></tr><tr><td align="left"><a href="https://paste.armbian.com/saqoqolehi">Cubietruck</a></td><td align="left">2023-08-08&nbsp;07:31:31</td><td align=right>edge</td><td align=right>6.4.8-sunxi</td><td align=right>330</td><td align=right>1006</td></tr><tr><td align="left"><a href="https://paste.armbian.com/zosaqubuyu">NanoPi R4S</a></td><td align="left">2023-08-08&nbsp;06:40:25</td><td align=right>current</td><td align=right>6.1.43-rockchip64</td><td align=right>924</td><td align=right>6470</td></tr><tr><td align="left"><a href="https://paste.armbian.com/osumijohuv">NanoPi R4S</a></td><td align="left">2023-08-08&nbsp;06:47:00</td><td align=right>edge</td><td align=right>6.4.8-rockchip64</td><td align=right>841</td><td align=right>6476</td></tr><tr><td align="left"><a href="https://paste.armbian.com/bamaxokula">Odroid N2</a></td><td align="left">2023-08-08&nbsp;06:37:21</td><td align=right>current</td><td align=right>6.1.43-meson64</td><td align=right>889</td><td align=right>8927</td></tr><tr><td align="left"><a href="https://paste.armbian.com/sisixozocu">Odroid N2</a></td><td align="left">2023-08-08&nbsp;06:42:22</td><td align=right>edge</td><td align=right>6.4.8-meson64</td><td align=right>860</td><td align=right>8644</td></tr><tr><td align="left"><a href="https://paste.armbian.com/foyuvubole">Orange Pi 3</a></td><td align="left">2023-08-08&nbsp;06:39:13</td><td align=right>legacy</td><td align=right>5.15.124-sunxi64</td><td align=right>790</td><td align=right>4488</td></tr><tr><td align="left"><a href="https://paste.armbian.com/rojurafela">Orange Pi 3</a></td><td align="left">2023-08-08&nbsp;06:46:14</td><td align=right>current</td><td align=right>6.1.43-sunxi64</td><td align=right>930</td><td align=right>4344</td></tr><tr><td align="left"><a href="https://paste.armbian.com/akikagenat">Orange Pi 3</a></td><td align="left">2023-08-08&nbsp;06:53:21</td><td align=right>edge</td><td align=right>6.4.8-sunxi64</td><td align=right>840</td><td align=right>4232</td></tr><tr><td align="left"><a href="n/a">NanoPi Neo 3</a></td><td align="left">2023-08-08&nbsp;06:32:22</td><td align=right>current</td><td align=right>n/a</td><td align=right>n/a</td><td align=right>n/a</td></tr><tr><td align="left"><a href="n/a">NanoPi Neo 3</a></td><td align="left">2023-08-08&nbsp;06:32:23</td><td align=right>edge</td><td align=right>n/a</td><td align=right>n/a</td><td align=right>n/a</td></tr><tr><td align="left"><a href="https://paste.armbian.com/omecojihog">Orange Pi Zero</a></td><td align="left">2023-08-08&nbsp;06:50:57</td><td align=right>legacy</td><td align=right>5.15.124-sunxi</td><td align=right>90</td><td align=right>2303</td></tr><tr><td align="left"><a href="https://paste.armbian.com/etuhavufax">Orange Pi Zero</a></td><td align="left">2023-08-08&nbsp;07:00:15</td><td align=right>current</td><td align=right>6.1.43-sunxi</td><td align=right>90</td><td align=right>2458</td></tr><tr><td align="left"><a href="https://paste.armbian.com/kupogefote">Orange Pi Zero</a></td><td align="left">2023-08-08&nbsp;07:09:52</td><td align=right>edge</td><td align=right>6.4.8-sunxi</td><td align=right>90</td><td align=right>2266</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ozuziqexef">Orange Pi Zero Plus</a></td><td align="left">2023-08-08&nbsp;06:46:34</td><td align=right>legacy</td><td align=right>5.15.124-sunxi64</td><td align=right>788</td><td align=right>2581</td></tr><tr><td align="left"><a href="https://paste.armbian.com/uhudojosug">Orange Pi Zero Plus</a></td><td align="left">2023-08-08&nbsp;06:56:16</td><td align=right>current</td><td align=right>6.1.43-sunxi64</td><td align=right>829</td><td align=right>2584</td></tr><tr><td align="left"><a href="https://paste.armbian.com/mulahegasu">Orange Pi Zero Plus</a></td><td align="left">2023-08-08&nbsp;07:05:26</td><td align=right>edge</td><td align=right>6.4.8-sunxi64</td><td align=right>780</td><td align=right>2582</td></tr><tr><td align="left"><a href="https://paste.armbian.com/amikuzopun">Orange Pi Zero2</a></td><td align="left">2023-08-08&nbsp;06:44:44</td><td align=right>current</td><td align=right>6.1.43-sunxi64</td><td align=right>778</td><td align=right>3111</td></tr><tr><td align="left"><a href="https://paste.armbian.com/holofawexo">Orange Pi Zero2</a></td><td align="left">2023-08-08&nbsp;06:54:33</td><td align=right>edge</td><td align=right>6.4.8-sunxi64</td><td align=right>800</td><td align=right>2877</td></tr><tr><td align="left"><a href="https://paste.armbian.com/awiwomivuy">Clearfog Pro</a></td><td align="left">2023-08-08&nbsp;06:43:23</td><td align=right>current</td><td align=right>6.1.43-mvebu</td><td align=right>717</td><td align=right>2228</td></tr><tr><td align="left"><a href="https://paste.armbian.com/etinabewub">Clearfog Pro</a></td><td align="left">2023-08-08&nbsp;06:49:25</td><td align=right>edge</td><td align=right>6.2.16-mvebu</td><td align=right>817</td><td align=right>2227</td></tr><tr><td align="left"><a href="https://paste.armbian.com/uqivabikac">ODROID M1</a></td><td align="left">2023-08-08&nbsp;06:41:49</td><td align=right>edge</td><td align=right>6.3.13-rk3568-odroid</td><td align=right>740</td><td align=right>5385</td></tr><tr><td align="left"><a href="https://paste.armbian.com/fokepuqulo">Tinker Board 2</a></td><td align="left">2023-08-08&nbsp;06:47:17</td><td align=right>current</td><td align=right>6.1.43-rockchip64</td><td align=right>860</td><td align=right>6789</td></tr><tr><td align="left"><a href="https://paste.armbian.com/uhigepirek">Tinker Board 2</a></td><td align="left">2023-08-08&nbsp;06:53:34</td><td align=right>edge</td><td align=right>6.4.8-rockchip64</td><td align=right>850</td><td align=right>6834</td></tr><tr><td align="left"><a href="https://paste.armbian.com/bowukesoro">Orange Pi 4 LTS</a></td><td align="left">2023-08-08&nbsp;06:40:02</td><td align=right>current</td><td align=right>6.1.43-rockchip64</td><td align=right>730</td><td align=right>5754</td></tr><tr><td align="left"><a href="https://paste.armbian.com/sidowavuva">Orange Pi 4 LTS</a></td><td align="left">2023-08-08&nbsp;06:46:32</td><td align=right>edge</td><td align=right>6.4.8-rockchip64</td><td align=right>830</td><td align=right>5315</td></tr><tr><td align="left"><a href="https://paste.armbian.com/azulijehew">Le potato</a></td><td align="left">2023-08-08&nbsp;06:47:23</td><td align=right>current</td><td align=right>6.1.43-meson64</td><td align=right>93</td><td align=right>3805</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ibomoremun">Le potato</a></td><td align="left">2023-08-08&nbsp;06:57:37</td><td align=right>edge</td><td align=right>6.4.8-meson64</td><td align=right>90</td><td align=right>3787</td></tr><tr><td align="left"><a href="https://paste.armbian.com/exuxaxewet">Banana Pi CM4IO</a></td><td align="left">2023-08-08&nbsp;06:36:09</td><td align=right>current</td><td align=right>6.1.43-meson64</td><td align=right>790</td><td align=right>9173</td></tr><tr><td align="left"><a href="https://paste.armbian.com/segisevala">Banana Pi CM4IO</a></td><td align="left">2023-08-08&nbsp;06:39:52</td><td align=right>edge</td><td align=right>6.4.8-meson64</td><td align=right>830</td><td align=right>8916</td></tr><tr><td align="left"><a href="https://paste.armbian.com/usisalosij">Banana Pi M5</a></td><td align="left">2023-08-08&nbsp;06:38:16</td><td align=right>current</td><td align=right>6.1.43-meson64</td><td align=right>841</td><td align=right>5556</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ejitomexas">Banana Pi M5</a></td><td align="left">2023-08-08&nbsp;06:43:55</td><td align=right>edge</td><td align=right>6.4.8-meson64</td><td align=right>840</td><td align=right>5556</td></tr><tr><td align="left"><a href="https://paste.armbian.com/iveyemujep">Khadas VIM2</a></td><td align="left">2023-08-08&nbsp;06:43:06</td><td align=right>current</td><td align=right>6.1.43-meson64</td><td align=right>852</td><td align=right>6163</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ohilogexar">Khadas VIM2</a></td><td align="left">2023-08-08&nbsp;06:53:47</td><td align=right>edge</td><td align=right>6.4.8-meson64</td><td align=right>852</td><td align=right>6063</td></tr><tr><td align="left"><a href="https://paste.armbian.com/humajuboci">Khadas VIM1</a></td><td align="left">2023-08-08&nbsp;06:42:15</td><td align=right>current</td><td align=right>6.1.43-meson64</td><td align=right>101</td><td align=right>3682</td></tr><tr><td align="left"><a href="https://paste.armbian.com/xozabujepe">Khadas VIM1</a></td><td align="left">2023-08-08&nbsp;06:51:27</td><td align=right>edge</td><td align=right>6.4.8-meson64</td><td align=right>89</td><td align=right>3680</td></tr><tr><td align="left"><a href="https://paste.armbian.com/oyolumodoc">Orange Pi R1 Plus LTS</a></td><td align="left">2023-08-08&nbsp;06:47:57</td><td align=right>current</td><td align=right>6.1.43-rockchip64</td><td align=right>509</td><td align=right>2087</td></tr><tr><td align="left"><a href="https://paste.armbian.com/veyeceputu">Orange Pi R1 Plus LTS</a></td><td align="left">2023-08-08&nbsp;07:00:21</td><td align=right>edge</td><td align=right>6.4.8-rockchip64</td><td align=right>564</td><td align=right>1887</td></tr><tr><td align="left"><a href="n/a">Rock 5B</a></td><td align="left">2023-08-08&nbsp;06:32:22</td><td align=right>legacy</td><td align=right>n/a</td><td align=right>n/a</td><td align=right>n/a</td></tr><tr><td align="left"><a href="https://paste.armbian.com/wupesuruqi">Orange Pi Zero Plus 2</a></td><td align="left">2023-08-08&nbsp;06:51:17</td><td align=right>legacy</td><td align=right>5.15.124-sunxi</td><td align=right>28</td><td align=right>2593</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ulenetamow">Orange Pi Zero Plus 2</a></td><td align="left">2023-08-08&nbsp;07:01:03</td><td align=right>current</td><td align=right>6.1.43-sunxi</td><td align=right>37</td><td align=right>2669</td></tr><tr><td align="left"><a href="https://paste.armbian.com/qehofesuru">Orange Pi Zero Plus 2</a></td><td align="left">2023-08-08&nbsp;07:11:10</td><td align=right>edge</td><td align=right>6.4.8-sunxi</td><td align=right>37</td><td align=right>2539</td></tr></table>
<!--END_SECTION:data-section-->

## Would you like to join spare hardware to this automated testings?

All you need to do is:

- deploy any latest Armbian image to hardware
- provide IP address
- [contact us](https://www.armbian.com/contact/)

Device has to be always on and easily accesible for you to re-image in case of failed upgrade.

## Development

- [Pull request](https://github.com/armbian/build/pulls)
- [Weekly developers meetings](https://forum.armbian.com/events/)
- [Forums for developers](https://forum.armbian.com/forum/4-advanced-users-development/)

## OS download

- [Download](https://www.armbian.com/download/)

## Support

- [Using Armbian](https://forum.armbian.com/forum/23-using-armbian/)

## Contact

- [Forums](https://forum.armbian.com) for Participate in Armbian
- IRC: `#armbian` on Libera.chat
- Discord: [https://discord.gg/armbian](https://discord.gg/armbian)
- Follow [@armbian](https://twitter.com/armbian) on Twitter, [Fosstodon](https://fosstodon.org/@armbian) or [LinkedIn](https://www.linkedin.com/company/armbian).
- Bugs: [issues](https://github.com/armbian/build/issues) / [JIRA](https://armbian.atlassian.net/jira/dashboards/10000)
- Office hours: [Wednesday, 12 midday, 18 afternoon, CET](https://calendly.com/armbian/office-hours)

## License

This software is published under the GPL-2.0 License license.
