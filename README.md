
##ChromeBook Crouton����

���������п� д���̳̣�ͨ��crouton��ʽר�Ÿ�arm�ܹ���chromeϵͳ��chrome����ƽ����ԣ���ݮ��ʹ����Ubuntuϵͳ��chrome os �ڲ���������ִ�е���һ�������Ļ�������crouton https://github.com/dnschneid/crouton
1. Unity��
Ubuntu 12.04 with Unity (2D)��sudo sh -e ~/Downloads/crouton -r precise -t unity -e
��arm�ܹ�unity���֧��12.04��
2.Xfce��
Ubuntu 14.04 with Xfce��sudo sh -e ~/Downloads/crouton -r trusty -t xfce -e
3. kubuntu�� sudo sh -e ~/Downloads/crouton -t kde 
������������sudo sh -e ~/Downloads/crouton -t touch,kde
���ƵĿ��԰�װgnome (GNOME Shell), cinnamon, lxde�ȷ��а汾������
�ο���1. http://www.linux.com/learn/tutorials/795730-how-to-easily-install-ubuntu-on-chromebook-with-crouton
2. http://www.webupd8.org/2013/12/install-ubuntu-on-your-chromebook-using.html
�����ʹ�ù���Դ��mirrors.ustc.edu.cn/ubuntu/ubuntu
�����նˣ��ڼ����ϰ�ctrl+alt+T �ο����ҵ�������簲װUbuntu14.04�Ļ� sudo sh -e ~/Downloads/crouton -r trusty -t xfce -e -m http://mirrors.ustc.edu.cn/ubuntu/ubuntu/
-m����˼��ָ��Դ��ַ
���ŵȴ���װ���������ն�����sudo startxfce�Ϳ�����
�ο���http://tieba.baidu.com/p/3490991713?pid=62200356240&cid=62661091999#62661091999


�ο�ԭ���� url https://github.com/dnschneid/crouton/raw/releases/$INSTALLER


crouton.proxy ����pac�����Ѿ��ϴ����ٶ��ƣ���������������notepad++����sublime�޸ġ��� �� 84�е� sed -i '/Execute the main script inline/ased -i '\''s/wget -O /wget -e "https_proxy=http:\\/\\/pac.xxxx.com:25\\/" -O /g'\'' $SCRIPTDIR/targets/audio' "$CACHEFILE" ��pac.xxx.com��ָ����������ַ���Լ�����ͨ��vps���������ip��ַҲ�С�
�ٶ��ƣ�http://pan.baidu.com/s/1bnIyMa7 ���룺jdj6