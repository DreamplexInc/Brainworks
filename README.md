# Brainworks
Простое IDE для создания C# проектов

> Внимание! Brainworks сейчас находится на стадии разработки

# Как писать свои плагины для Brainworks?
## Примерный код (для консольных плагинов, без UI) :
```c#
using System;
using System.Threading;
using System.Collections;

static void Main(string[] args)
{
  Console.WriteLine("Brainworks работает!");
  Brainworks.StopProcess();
}
```
## или же на C/C++ : 
```c++
#include <string>
using namespace std;
int main()
{
  string inp;
  cout << "Brainworks is working!" << endl;
  cin >> inp;
}
```
> Внимание! Вызов метода "Brainworks.StopProcess();" обязательна, иначе ваш плагин никогда не выключится и будет работать в фоне.
