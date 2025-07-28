Preparar Kali para trabajar

# Actualización del sistema
sudo apt-get update && sudo apt-get upgrade -y

# Instalación de ZSH, Curl, Git y Terminător
sudo apt-get install zsh curl git terminator -y

# Instalación de Oh My Zsh
echo "y" | sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)" 
chsh -s $(which zsh)

# Instalación del tema Powerlevel10k
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git \ ${ZSH_CUSTOM: -$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

# Cambiar el tema en .zshrc
sed -i 's/ZSH_THEME="robbyrussell"/ZSH_THEME="powerlevel10k\/powerlevel10k"/* ~/.zshrc

# Instalación de plugins para ZSH
sudo apt install zsh-autosuggestions zsh-syntax-highlighting -y

# Activación de plugins en .zshrc
echo "# Plugins" >> ~/.zshrc
echo "source /usr/share/zsh-autosuggestions/zsh-autosuggestions.zsh" >> ~/.zshrc
echo "source /usr/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ~/.zshrc

# Descarga e instalación de fuentes MesloLGS (requeridas por Powerlevel10k)
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf 
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf 
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf 
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf 

sudo mv MesloLGS\ Nf\ *.ttf/usr/local/share/fonts/
fc-cache -fv

#Salir para que los cambios tengan efectos
exit