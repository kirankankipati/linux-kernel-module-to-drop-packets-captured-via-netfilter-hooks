Sample Linux Kernel Module to drop packets (i.e sk_buff instance) captured via netfilter hooks as discussed in my YouTube video. When you want to drop packets in your custom netfilter hooks make sure you never do a manual kfree_skb(skb) API call. Since it is anyway performed once the flow of the code moves out of your kernel module netfilter hook. All you need to do is to return NF_DROP to drop gracefully the desired packet.

For more details kindly refer:
my Website article - The Linux Channel - https://thelinuxchannel.org/2023/12/linux-kernel-module-to-drop-packets-captured-via-netfilter-hooks/
my YouTube video - https://youtu.be/zioet4kGwDE

I also conduct sessions/classes on Systems and Network Software Programming, Linux Kernel Programming and Architecture. Kindly follow the link below:
https://thelinuxchannel.org/courses/

If you have any queries or anything to discuss further on Linux Kernel Programming and writing Kernel modules kindly feel free to contact me. Kindly follow the link below:
https://thelinuxchannel.org/contact/
