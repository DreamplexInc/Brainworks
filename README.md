# Brainworks
Простое IDE для создания C# проектов

> Внимание! Brainworks не работает с форматами Microsoft Office!

> Программа Brainworks на данный момент только умеет шифровать данные, которые хранятся
> в формате txt

# Как писать свои плагины для Brainworks?
Примерный код (для консольных плагинов, без UI) :
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
> Внимание! Вызов метода "Brainworks.StopProcess();" обязательна, иначе ваш плагин никогда не выключится и будет работать в фоне.
