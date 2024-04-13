vmware_tools安装
软件与更新中更换国内源
sudo apt update
sudo apt upgrade

# 拖拽
sudo apt install gnome-shell-extension-prefs
sudo apt install nemo

application的extensions把Desktop iconsNG关闭
application选择startup application preference，添加：
name: nemo desktop
command: nemo-desktop
comment: nemo desktop

# 桌面美化
挑选下载主题：https://www.gnome-look.org/browse/
https://github.com/vinceliuice/Orchis-theme
https://github.com/vinceliuice/Canta-theme/tree/master
github下载主题相关文件并安装
安装tweak: sudo apt install gnome-tweaks
sudo reboot
gnome-tweaks，设置主题和图标
安装chrome：
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i google-chrome-stable_current_amd64.deb
sudo apt-get -f install
使用 GNOME Shell 扩展：extensions.gnome.org
google插件安装：GNOME Shell 集成
安装本地连接器：sudo apt install chrome-gnome-shell
安装扩展：Apps Menu, Clipboard Indicator, Extension List, Net Speed, Removable Drive Menu, User Themes, Vitals, dash to dock

安装anaconda
sudo vim ~/.bashrc
export PATH=/home/dpw/anaconda3/bin:$PATH
source ~/.bashrc

pip源
mkdir ~/.pip
sudo vim ~/.pip/pip.conf
# 将以下内容添加到~/.pip/pip.conf
[global]
index-url = http://mirrors.aliyun.com/pypi/simple/

[install]
trusted-host=mirrors.aliyun.com

安装pycharm
sudo tar xzf pycharm-*.tar.gz -C ~/
cd /usr/share/applications/
sudo gedit pycharm.desktop

[Desktop Entry]
Type=Application
Name=Pycharm    
GenericName=Pycharm3                                                    
Comment=Pycharm3:The Python IDE                                     
Exec=/home/sjx/pycharm-2023.3.4/bin/pycharm.sh
Icon=/home/sjx/pycharm-2023.3.4/bin/pycharm.png
Terminal=pycharm
Categories=Pycharm;

拖到桌面
破解pycharm
汉化

中文输入：
sudo apt install ibus-pinyin
ibus-setup

安装向日葵






