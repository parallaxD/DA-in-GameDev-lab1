# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #1 выполнил(а):
- Куплевацкий Денис Игоревич
- РИ220931
Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | * | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 2.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 3.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.
- ✨Magic ✨

## Цель работы
Установить необходимое программное обеспечение, которое пригодится для создания интеллектуальных моделей на Python. Рассмотреть процесс установки игрового движка Unity для разработки игр.

## Задание 1
### Написать программу Hello World на Python с запуском в Jupiter Notebook.
Ход работы:
- С сайта https://www.anaconda.com был установлен дистрибутив Anaconda. Через anaconda-navigator был запущен инструмент Jupyter Notebook. В окне браузера была создана папка DataAnalysis и файл HelloWorld.ipynb внутри неё.
В файл была вписана команда **print('Hello World')**

![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/11c8d099-5c07-4d7b-9c7b-41e8b01f7f41)
![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/eb2735d0-dc29-457c-b3d0-04b010630aeb)
![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/17a4dfca-e274-47cc-aac9-8fc41d05964f)


## Задание 2
### Написать программу Hello World на C# с запуском на Unity.

- С сайта https://unity.com был установлен игровой движок **Unity** и приложение **Unity Hub**.
- Создан пустой 3D-проект под названием Data Analysis In GameDev.
- На сцене был создан пустой объект под названием **HelloWorldWriter**
- Была создана папка **Scripts** и скрипт в ней под названием **HelloWorldWriter**
- В методе Start() был реализован вывод сообщения "Hello World" в консоль Unity с помощью класса Debug и метода Log().

![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/649391e3-0aea-41fa-b317-1bcea20d6e1b)


```C#

using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class HelloWorldWriter : MonoBehaviour
{
    void Start()
    {
        Debug.Log("Hello World");
    }
}

```

## Задание 3
### Какова роль параметра Lr? Ответьте на вопрос, приведите пример выполнения кода, который подтверждает ваш ответ. В качестве эксперимента можете изменить значение параметра.

- Перечисленные в этом туториале действия могут быть выполнены запуском на исполнение скрипт-файла, доступного [в репозитории](https://github.com/Den1sovDm1triy/hfss-scripting/blob/main/ScreatingSphereInAEDT.py).
- Для запуска скрипт-файла откройте Ansys Electronics Desktop. Перейдите во вкладку [Automation] - [Run Script] - [Выберите файл с именем ScreatingSphereInAEDT.py из репозитория].

```py

import ScriptEnv
ScriptEnv.Initialize("Ansoft.ElectronicsDesktop")
oDesktop.RestoreWindow()
oProject = oDesktop.NewProject()
oProject.Rename("C:/Users/denisov.dv/Documents/Ansoft/SphereDIffraction.aedt", True)
oProject.InsertDesign("HFSS", "HFSSDesign1", "HFSS Terminal Network", "")
oDesign = oProject.SetActiveDesign("HFSSDesign1")
oEditor = oDesign.SetActiveEditor("3D Modeler")
oEditor.CreateSphere(
	[
		"NAME:SphereParameters",
		"XCenter:="		, "0mm",
		"YCenter:="		, "0mm",
		"ZCenter:="		, "0mm",
		"Radius:="		, "1.0770329614269mm"
	], 
)

```

## Выводы

Абзац умных слов о том, что было сделано и что было узнано.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
