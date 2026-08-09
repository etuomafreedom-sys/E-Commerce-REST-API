# E-Commerce-REST-API
# 🛒 E-Commerce Storefront REST API — Django REST Framework

A lightweight, scalable **RESTful Web API** built with **Django REST Framework (DRF)** for managing e-commerce product catalogs. This project demonstrates model serialization, automated URL routing, and clean CRUD (Create, Read, Update, Delete) operations using DRF `ModelViewSet`.

---

## ✨ Features & Architecture

- 📦 **Complete Product CRUD:** Single viewset supporting list, retrieve, create, update, and delete actions.
- ⚡ **Model Serialization:** Automated JSON conversion and validation using `serializers.ModelSerializer`.
- 🔌 **RESTful Endpoints:** Standardized HTTP responses (`GET`, `POST`, `PUT`, `PATCH`, `DELETE`).
- 🛠️ **DRF Browsable API:** Built-in web view for testing endpoints directly in the browser.

---

## 🏗️ API Architecture

### `serializers.py`
```python
from rest_framework import serializers
from .models import Product

class ProductSerializer(serializers.ModelSerializer):
    class Meta:
        model = Product
        fields = '__all__'
