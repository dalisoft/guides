# Parallels Desktop

```bash
cp /Library/Preferences/Parallels/licenses.json ~/Downloads/licenses.json # backup
sudo mv ~/Downloads/licenses.json /Library/Preferences/Parallels/licenses.json # restore

sudo su # Enter your password and then:
echo $(sed 's/202[0-9]-[0-1][0-9]-[0-3][0-9]/2099-07-15/g' /Library/Preferences/Parallels/licenses.json;) > /Library/Preferences/Parallels/licenses.json;
```

## Network fix

```bash
sudo sed -i '' 's/<UseKextless>\([[:digit:]_-]\{1,\}\)<\/UseKextless>/<UseKextless>0<\/UseKextless>/g' /Library/Preferences/Parallels/network.desktop.xml && grep '<UseKextless>' /Library/Preferences/Parallels/network.desktop.xml
```

## USB fix

```bash
sudo sed -i '' 's/<Usb>\([[:digit:]_-]\{1,\}\)<\/Usb>/<Usb>1<\/Usb>/g' /Library/Preferences/Parallels/dispatcher.desktop.xml && grep '<Usb>' /Library/Preferences/Parallels/dispatcher.desktop.xml
```

## Windows 10/11 Activation

<details>

<summary><b>OLD; NOT WORKS! NOT RECOMMENDED!</b></summary>

<https://msguides.com/windows-11>

```ps
slmgr/ipk W269N-WFGWX-YVC9B-4J6C9-T83GX
slmgr /skms kms.digiboy.ir
slmgr /ato
# or
slmgr /ipk TX9XD-98N7V-6WMQ6-BX7FG-H8Q99
slmgr /skms s8.uk.to
slmgr /ato
```

</details>
