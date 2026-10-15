# Автоматизированная система учёта и формирования договорной документации с интеграцией с 1С и ЭДО

![.NET](https://img.shields.io/badge/.NET-8.0%2F9.0-512BD4?style=flat&logo=dotnet)
![C#](https://img.shields.io/badge/C%23-12.0-239120?style=flat&logo=csharp)
![WPF](https://img.shields.io/badge/UI-WPF%20%2F%20MaterialDesign-0078D4?style=flat)
![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-4169E1?style=flat&logo=postgresql)
![License](https://img.shields.io/badge/License-MIT-green.style=flat)

Выпускная квалификационная работа (дипломный проект) по разработке десктопной системы автоматизации договорного учёта, генерации документов и интеграции с корпоративными сервисами.

---

## 📌 О проекте

Проект предназначен для автоматизации полного цикла работы с договорной документацией на коммерческом предприятии:
1. Ведение базы данных контрагентов и договоров.
2. Автоматическое формирование документов по `.docx`-шаблонам без необходимости использования MS Office.
3. Двусторонняя синхронизация реквизитов и документов с **1С:Предприятие** через REST API / OData.
4. Отправка и отслеживание статусов подписания документов в системах **ЭДО** (Контур.Диадок / СБИС).

---

## 🛠 Стек технологий

* **Язык и платформа:** C# (.NET 8.0 / .NET 9.0)
* **Пользовательский интерфейс (UI):** WPF, MVVM (`CommunityToolkit.Mvvm`), MaterialDesignInXamlToolkit
* **База данных и ORM:** PostgreSQL, Entity Framework Core (Code First)
* **Генерация документов:** DocumentFormat.OpenXML / DocX (автономное формирование документов `.docx`/`.pdf` без зависимости от MS Office)
* **Интеграции:**
  * **1С:** REST API / OData (с использованием `HttpClient`)
  * **ЭДО:** REST API / SDK (Контур.Диадок / СБИС)
* **Архитектурный подход:** Clean Architecture (Domain, Application, Infrastructure, UI)

---

## 🏗 Архитектура приложения

Проект построен по принципам **Clean Architecture** и паттерну **MVVM** для обеспечения высокой модульности и тестируемости

