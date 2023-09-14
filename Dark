#!/bin/bash
plain='\033[0m'
red='\e[31m'
yellow='\e[33m' 
gray='\e[90m'   
green='\e[92m'  
blue='\e[94m'   
magenta='\e[95m'
cyan='\e[96m'   
none='\e[0m'    
username="yyp26"
password="yyp26"
sshlimiter="1500"
servermessage="<h3><font color='red'>
◈──────⪧ Servers Messages ⪦ ───────◈
</font></h3>
<h4><font color='cyan'>
Mytel GCP Public SSH Key
</font></h4>
<h4><font color='cyan'>
Used Count ◈──⪧ 1,500
</font></h4>
<h3><font color='red'>
◈──────⪧  SSH Public Key ⪦ ───────◈
</font></h3>"
[[ $EUID -ne 0 ]] && echo -e "${red}Error: ${plain} You must use root user to run this script!\n" && exit 1

sed -i 's/#\?AllowTcpForwarding .*/AllowTcpForwarding yes/' /etc/ssh/sshd_config && sed -i 's/#\?PasswordAuthentication .*/PasswordAuthentication yes/' /etc/ssh/sshd_config && sed -i 's/#\?Banner .*/Banner \/etc\/ssh\/gcp_404/' /etc/ssh/sshd_config && /etc/init.d/ssh restart;
echo "$servermessage" | tee /etc/ssh/gcp_404 >/dev/null
final=$(date "+%Y-%m-%d" -d "+$dias days")
gui=$(date "+%d/%m/%Y" -d "+$dias days")
pass=$(perl -e 'print crypt($ARGV[0], "password")' $password)
useradd -e $final -M -s /bin/false -p $pass $username >/dev/null
echo "$password" >/etc/$username
echo "$username:$password" | chpasswd
echo "$username $sshlimiter" >>/root/usuarios.db
IP=$(wget -qO- ipv4.icanhazip.com)
echo ""
echo -e "\033[1;32m  🥰🥰🥰🥰🥰💯💯💯🥰🥰🥰🥰🥰
echo -e "\033[1;32m◈─────────────────────────────────◈"
echo -e "\033[1;32m    ©️ 🐉 Dark VPS MANAGER SCRIPT 🐉  " 
echo -e "\033[1;32m◈─────────────────────────────────◈"
echo ""
echo -e "\033[1;37m◈─────⪧ SSH ACCOUNT ⪦─────◈"
echo ""
echo -e "\033[1;32m◈─ᗚ Host / IP   • ๛   \033[1;31m$IP"
echo -e "\033[1;32m◈─ᗚ Port        • ๛   \033[1;31m22"
echo -e "\033[1;32m◈─ᗚ Username    • ๛   \033[1;31m$username"
echo -e "\033[1;32m◈─ᗚ Password    • ๛   \033[1;31m$password"
echo -e "\033[1;32m◈─ᗚ Login Limit • ๛   \033[1;31m$sshlimiter"
echo -e "\033[1;32m◈─ᗚ Expire Date • ๛   \033[1;31m$gui"
echo ""
echo -e "\033[1;37m◈────⪧  Y.Y.P SSH Servers ⪦────◈"
echo -e "\033[1;32m[-] ═──────────────────⪧◇⪦─────────────────═                                            echo -e "\033[1;32m◈─ᗚ Login Limit • ๛   \033[1;31m$sshlimiter"
cho -e "\033[1;32m         ࿂ Login Limit • ๛   \033[1;31m$sshlimiter"
echo -e "\033[1;32m.       ࿂ Expire Date • ๛   \033[1;31m$gui"
echo ""
echo -e "\033[1;32m[-] ═──────────────────⪧◇⪦─────────────────═                                           
echo -e "\033[1;32m›☬[•] SCRIPTS ═◇ DARKSSH ◇═ [•]☬ 
echo ""
echo "──⪧═───────◇───────═⪦──"
printf " Y . Y . P  S S H \n"
echo "──⪧═───────◇───────═⪦──"
echo ""

echo -e "${yellow}▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬ ${plain}"
echo -e "${cyan}      I want time to stop                                                     ${plain}"
echo -e "${cyan}      Because I always want to be by your side                                ${plain}"
echo -e "${cyan}        ⣠⣶⣶⣦⡀                                                                ${plain}"
echo -e "${cyan}⠀⠀⠀⠀⠀⠀⢰⣿⣿⣿⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀                                                  ${plain}"
echo -e "${cyan}⠀⠀⠀⠀⠀⠀⠀⠻⣿⣿⡿⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀                                                  ${plain}"
echo -e "${cyan}⠀⠀⠀⠀⠀⠀⣴⣶⣶⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀                                                  ${plain}"
echo -e "${cyan}⠀⠀⠀⠀⠀⣸⣿⣿⣿⣿⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀                                                  ${plain}"
echo -e "${cyan}⠀⠀⠀⠀ ⣿ Me.                                                                   ${plain}"
echo -e "${cyan}⠀⠀⠀⠀⣼⣿⣿⣿⡿⣿⣿⣆⠀⠀⠀⠀⠀⠀⣠⣴⣶⣤⡀⠀                                                 ${plain}"
echo -e "${cyan}⠀⠀⠀⢰⣿⣿⣿⣿⠃⠈⢻⣿⣦⠀⠀⠀ ⠀⣸You⣿⣷⠀                                                ${plain}"
echo -e "${cyan}⠀⠀⠀⠘⣿⣿⣿⡏⣴⣿⣷⣝⢿⣷⢀⠀⢀⣿⣿⣿⣿⡿⠋⠀                                                  ${plain}"
echo -e "${cyan}⠀⠀⠀⠀⢿⣿⣿⡇⢻⣿⣿⣿⣷⣶⣿⣿⣿⣿⣿⣷⠀⠀⠀⠀                                                  ${plain}"
echo -e "${cyan}⠀⠀⠀⠀⢸⣿⣿⣇⢸⣿⣿⡟⠙⠛⠻⣿⣿⣿⣿⡇⠀⠀⠀⠀                                                  ${plain}"
echo -e "${cyan}⣴⣿⣿⣿⣿⣿⣿⣿⣠⣿⣿⡇⠀⠀⠀⠉⠛⣽⣿⣇⣀⣀⣀⠀                                                  ${plain}"
echo -e "${cyan}⠙⠻⠿⠿⠿⠿⠿⠟⠿⠿⠿⠇⠀⠀⠀⠀⠀⠻⠿⠿⠛⠛⠛⠃                                                  ${plain}"
echo -e "${red}          S . S . H  A C C O U N T                                             ${plain}"
echo -e "${green}      ࿂ ═─────────⪧.  Now the thing is ready to use.  ⪦─────────═        ${plain}"
echo -e "${yellow}▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬▬ ${plain}"

echo -e "${cyan} Y.Y.P SSH  😎 ${plain}"
