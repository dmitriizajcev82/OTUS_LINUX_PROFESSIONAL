# VAGRANT
Vagrant — продукт компании HashiCorp, специализирующейся на инструментах для автоматизации разработки и эксплуатации. Он позволяет создавать и конфигурировать легковесные, повторяемые и переносимые окружения для разработки.

Для работы с Vagrant необходимо установить vagrant. Для примеры взять ОС GNU Linux.

~~~shell
# deb пакеты

$ curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -
$ sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
$ sudo apt-get update && sudo apt-get install vagrant

# yum пакеты

$ sudo yum install -y yum-utils
$ sudo yum-config-manager --add-repo https://rpm.releases.hashicorp.com/RHEL/hashicorp.repo
$ sudo yum -y install vagrant
~~~

## Проверить версию vagrant

~~~shell
vagrant --version
~~~

## Запуск vagrant 

~~~shell
vagrant up
~~~

## Подключиться к виртальной машине

~~~shell
vagrant ssh
~~~

## Остановить виртуальную машину

~~~shell
vagant halt
~~~

## Удалить виртуальную машину

~~~shell
vagrant destroy
~~~

## Пример vagrant file

~~~shell
Vagrant.configure(2) do |config| # объект конфигурации
 config.vm.define "vm-1" do |srv| # объект виртуальной машины
 srv.vm.box = "debian/12.1" # задали box (VM image)
 end
end
~~~

## Команды управления виртуальной машины

~~~shell 
vagrant up # старт и создание VM из файла описания
vagrant status # проверим состояние
vagrant global-status # проверим состояние всех VM
vagrant ssh # подключение к VM
vagrant ssh name # подключение к VM по имени
vagrant ssh-config # приватный ключ, настройки подключения
vagrant halt # остановка
vagrant destroy # удаление VM вместе с данными приложений
~~~

