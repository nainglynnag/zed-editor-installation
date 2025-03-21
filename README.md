# Install Zed Editor on Ubuntu

Zed is a fast, collaborative code editor. I hope this guide provides you a little help step-by-step instructions for installing Zed on **Ubuntu Linux**.


## 🔽 Installation Steps

### 1️⃣ Open a terminal and run the following command
To install the stable version:

```sh
curl -f https://zed.dev/install.sh | sh
```

If you'd like to test the new features earlier, run the following command to install the preview version:

```sh
curl -f https://zed.dev/install.sh | ZED_CHANNEL=preview sh
```

![Install Zed in terminal](./images/zedinstall.img)

### 2️⃣ Launch Zed
Once installed, open Zed from the terminal:

```sh
zed
```

Or launch it from the application menu.
Zed editor window will be appeared as follows:

![Open Zed](./images/zedwindow.img)

### 3️⃣ (Optional) Create a Desktop Shortcut
To add Zed to the applications list, create a `.desktop` entry:

```sh
nano ~/.local/share/applications/zed.desktop
```

Add the following content:

```ini
[Desktop Entry]
Name=Zed
Exec=zed
Icon=/usr/share/icons/hicolor/256x256/apps/zed.png
Type=Application
Categories=Development;
```

Save and close (`CTRL+X`, `Y`, `Enter`). Then, refresh the application menu:

```sh
gtk-update-icon-cache ~/.local/share/icons/hicolor/
```

---

## ✅ Verification
To ensure Zed is installed correctly, run:

```sh
zed --version
```

You should see output similar to:

```sh
Zed version X.Y.Z
```

---

## 🛠 Official Docs
If you have any problem, you can also check it on the ![Zed Editor](https://zed.dev/docs/getting-started) official website.


## 📌 Uninstalling Zed
To remove Zed, run:

```sh
sudo apt remove zed
```

And delete the `.deb` file if needed:

```sh
rm zed.deb
```

---

### 🎉 Enjoy Coding with Zed!

