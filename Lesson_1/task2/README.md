# Обновить ядро операционной системы Linux
Текущая операционная система.
```shell
 lsb_release -r
```
<details>
    <a href="https://freeimage.host/i/JYltgna"><img src="https://iili.io/JYltgna.md.png" alt="JYltgna.md.png" border="0"></a><br /><a target='_blank' href='https://freeimage.host/'></a><br>
</details>
Версия ядра до обновления
<details>
  <a href="https://freeimage.host/i/JYlDCMb"><img src="https://iili.io/JYlDCMb.md.png" alt="JYlDCMb.md.png" border="0"></a>
</details>
Ядро операционной системы обновлял с помощью программного обеспечения mainline.
Основной установщик ядра Ubuntu имеет свою официальную панель запуска PPA, которую нужно импортировать. В терминале запустите следующую команду:

```shell
 sudo add-apt-repository ppa:cappelikan/ppa
```
Далее проверим обновления и установим ПО.

```shell
sudo apt update && apt install mainline
```
Проверим список доступных ядер операционной системы Linux

```shell
mainline --list
```
<details>
  <a href="https://freeimage.host/i/JYlb0Xe"><img src="https://iili.io/JYlb0Xe.md.png" alt="JYlb0Xe.md.png" border="0"></a>
</details>
Установим последнее доступное ядро

```shell
mainline install 6.7
```
<details>
  <a href="https://freeimage.host/i/JYlbUrv"><img src="https://iili.io/JYlbUrv.md.png" alt="JYlbUrv.md.png" border="0"></a><br /><a target='_blank' href='https://freeimage.host/'></a><br />
</details>

Обновленное ядро операционной системы Linux
<details>
  <a href="https://freeimage.host/i/JYlmuZF"><img src="https://iili.io/JYlmuZF.md.png" alt="JYlmuZF.md.png" border="0"></a>
</details>
