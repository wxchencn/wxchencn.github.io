# zsh & oh my zsh

for 'mqw' and 'jiss'

---

## install zsh & oh my zsh

- 使用zsh代替bash，ohmyzsh是zsh的配置工具

- 后面使用中所有对 ‘.bashrc’ 的修改，都应改为对 '.zshrc' 的修改

### install zsh

```
sudo apt install zsh
```

### install oh my zsh

```shell
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

or

```shell
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

or

```shell
wget https://github.com/ohmyzsh/ohmyzsh/blob/master/tools/install.sh
chmod 755 install.sh
./install.sh
```



## install plugin

### zsh-syntax-highlighting

效果：shell 语法高亮，正确为绿色

**install：**

```shell
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

**setup：**

```shell
zshconfig
修改为： plugins = (git zsh-syntax-highlighting)
```

### zsh-autosuggestions

效果：命令智能提示，右箭头‘->’补全

**install：**

```shell
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

**setup：**

```shell
zshconfig
修改为： plugins = (git zsh-autosuggestions)
```

