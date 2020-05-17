# orbital_plot

## Installing Vesta

Download Vesta from this link: [Download](https://jp-minerals.org/vesta/archives/3.5.2/VESTA-gtk3.tar.bz2)

**Installing Commands**
```shell
cd ~/Downloads
tar -xvf VESTA-gtk3.tar.bz2
sudo mv ./VESTA-gtk3 /opt
sudo cp /opt/libVESTA.so /usr/local/lib
sudo chown root:root  /usr/local/lib/libVESTA.so
sudo chmod 775 /usr/local/lib/libVESTA.so
sudo ldconfig -v
```

**Creating Desktop Entry**

```shell
touch vesta.desktop
echo "[Desktop Entry]" >> ./vesta.desktop
echo "Version=3.5.2" >> ./vesta.desktop
echo "Type=Application" >> ./vesta.desktop
echo "Name=Vesta" >> ./vesta.desktop
echo "Comment=" >> ./vesta.desktop
echo "Exec=/opt/VESTA-gtk3/VESTA-gui" >> ./vesta.desktop
echo "Icon=/opt/VESTA-gtk3/img/logo.png" >> ./vesta.desktop
echo "Path=" >> ./vesta.desktop
echo "Terminal=false" >> ./vesta.desktop
echo "StartupNotify=false" >> ./vesta.desktop 
sudo mv ./vesta.desktop /usr/share/applications/
```


