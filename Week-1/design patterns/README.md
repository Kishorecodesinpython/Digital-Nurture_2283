
# Singleton Pattern in C#

This project demonstrates the **Singleton Design Pattern** in C#, using a simple `Logger` class.

## 🔍 Problem Scenario

In many real-world applications, you often need only one instance of a class to coordinate actions across the system. For example, a logging utility should use the same logger object globally for consistent logging behavior. The Singleton pattern ensures that only one instance of the class is created and provides a global access point to it.

---

## 🏗️ Project Structure

- `Logger.cs` — Contains the singleton `Logger` class.
- `Program.cs` — Demonstrates how multiple calls to `Logger.GetInstance()` return the same object.

---

## 📂 How It Works

- `Logger` is a class with:
  - A **private static field** `instance` holding the single object.
  - A **private constructor** to prevent external instantiation.
  - A **public static method** `GetInstance()` to control object creation and return the same instance every time.

---
# 🏭 Factory Method Pattern in C#

This project demonstrates the **Factory Method Design Pattern** using a document management system that creates different types of documents (Word, PDF, and Excel) dynamically via dedicated factory classes.

---

## 📌 Problem Scenario

You are building a document management system that needs to support multiple types of documents. Directly using `new` to instantiate each document type violates the principle of loose coupling and makes your code less flexible and harder to extend.

To solve this, we apply the **Factory Method Pattern** — allowing subclasses to decide which class to instantiate while keeping the creation logic abstracted from the client code.

---

## 🧱 Project Structure

```bash
FactoryMethodPatternExample/
│
├── IDocument.cs               # Interface for all documents
├── WordDocument.cs           # Word document implementation
├── PdfDocument.cs            # PDF document implementation
├── ExcelDocument.cs          # Excel document implementation
│
├── DocumentFactory.cs        # Abstract factory class
├── WordDocumentFactory.cs    # Factory for WordDocument
├── PdfDocumentFactory.cs     # Factory for PdfDocument
├── ExcelDocumentFactory.cs   # Factory for ExcelDocument
│
└── Program.cs                # Main method for testing document creation


