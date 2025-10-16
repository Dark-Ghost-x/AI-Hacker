# AI-Hacker

```markdown
# AI-Powered Vulnerability Scanner Framework  
# چارچوب اسکنر آسیب‌پذیری هوشمند

![Framework Architecture](https://img.shields.io/badge/Version-2.0.0-blue.svg)
![Python](https://img.shields.io/badge/Python-3.8+-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Status](https://img.shields.io/badge/Status-Extensible%20Template-orange.svg)

## 📖 فهرست مطالب / Table of Contents
- [معرفی / Introduction](#معرفی--introduction)
- [ویژگی‌های کلیدی / Key Features](#ویژگیهای-کلیدی--key-features)
- [معماری فریمورک / Framework Architecture](#معماری-فریمورک--framework-architecture)
- [نصب و راه‌اندازی / Installation](#نصب-و-راهاندازی--installation)
- [استفاده سریع / Quick Start](#استفاده-سریع--quick-start)
- [توسعه و سفارشی‌سازی / Development & Customization](#توسعه-و-سفارشیسازی--development--customization)
- [API Documentation](#api-documentation)
- [مثال‌های توسعه / Development Examples](#مثالهای-توسعه--development-examples)
- [مشارکت / Contributing](#مشارکت--contributing)
- [مجوز / License](#مجوز--license)

## معرفی / Introduction

### فارسی
**چارچوب اسکنر آسیب‌پذیری هوشمند** یک پلتفرم ماژولار و کاملا قابل توسعه برای اسکن امنیتی است. این فریمورک به گونه‌ای طراحی شده که توسعه‌دهندگان می‌توانند به راحتی:

- مدل‌های هوش مصنوعی خود را اضافه کنند
- داده‌های آموزشی سفارشی از طریق API متصل کنند
- انواع جدید آسیب‌پذیری پیاده‌سازی کنند
- تکنیک‌های اسکن جدید توسعه دهند

این پروژه به عنوان یک **قالب خالی** شروع می‌شود و شما آن را با نیازهای خاص خود پر می‌کنید.

### English
**AI-Powered Vulnerability Scanner Framework** is a modular and fully extensible platform for security scanning. This framework is designed so developers can easily:

- Add their own AI models
- Connect custom training data via APIs
- Implement new vulnerability types
- Develop new scanning techniques

This project starts as an **empty template** and you fill it with your specific needs.

##  ویژگی‌های کلیدی / Key Features

### قابلیت توسعه‌پذیری / Extensibility
| ویژگی / Feature | توضیحات / Description |
|----------------|----------------------|
| **ماژولار** / Modular | معماری مبتنی بر کامپوننت‌های مستقل |
| **پلاگین‌بیس** / Plugin-based | اضافه کردن قابلیت‌های جدید بدون تغییر هسته |
| **اینترفیس‌محور** / Interface-driven | پیاده‌سازی آسان با رابط‌های استاندارد |

### 🤖 پشتیبانی از مدل‌های هوش مصنوعی / AI Model Support
| نوع مدل / Model Type | قابلیت‌ها / Capabilities |
|---------------------|-------------------------|
| **مدل‌های ML** / ML Models | KNN, Random Forest, SVM, etc. |
| **مدل‌های NLP** / NLP Models | GPT, BERT, Transformers, etc. |
| **مدل‌های سفارشی** / Custom Models | هر مدل پایتونی با رابط استاندارد |

### 🌐 اتصال داده‌های آموزشی / Training Data Connectivity
| منبع داده / Data Source | پشتیبانی / Support |
|------------------------|-------------------|
| **APIهای خارجی** / External APIs | RESTful APIs, GraphQL |
| **فایل‌های محلی** / Local Files | JSON, TXT, CSV, XML |
| **پایگاه‌داده** / Databases | SQL, NoSQL |

## 🏗 معماری فریمورک / Framework Architecture

```
```
┌─────────────────────────────────────────────────────────────┐
│لایه نمایش / Presentation Layer          │
├─────────────────────────────────────────────────────────────┤
│CLI Interface • REST API • Web Dashboard                   │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│لایه هسته / Core Layer                   │
├─────────────────────────────────────────────────────────────┤
│VulnerabilityScannerFramework (هماهنگ‌کننده اصلی)          │
│• Model Registry • Scanner Registry • API Registry         │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│لایه سرویس‌ها / Services Layer                  │
├─────────────────────────────────────────────────────────────┤
│┌─────────────┐  ┌─────────────┐  ┌─────────────┐         │
││   AI Models │  │  Scanners   │  │ Data APIs   │         │
││   • ML      │  │  • SQLi     │  │ • External  │         │
││   • NLP     │  │  • RCE      │  │ • Local     │         │
││   • Custom  │  │  • XSS      │  │ • Database  │         │
│└─────────────┘  └─────────────┘  └─────────────┘         │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│لایه ابزارها / Utilities Layer                    │
├─────────────────────────────────────────────────────────────┤
│HTTP Client • WAF Evasion • Parameter Discovery • Logging  │
└─────────────────────────────────────────────────────────────┘
```

```

##  نصب و راه‌اندازی / Installation

### پیش‌نیازها / Prerequisites
```
# Python 3.8 or higher
```
```
python --version
```
```

# pip package manager
```
```
pip --version
```

نصب بسته‌ها / Installing Dependencies

```
# Clone the repository
```
```
git clone https://github.com/Dark-Ghost-x/AI-Hacker.git
cd AI-Hacker
```
```

🔧 توسعه و سفارشی‌سازی / Development & Customization

📋 مراحل توسعه / Development Steps

1. اضافه کردن مدل هوش مصنوعی جدید / Adding New AI Model

```python
from framework import MLModel

class MyCustomModel(MLModel):
    def load_model(self, model_path=None):
        # پیاده‌سازی بارگذاری مدل
        self.model = load_your_model(model_path)
        
    def train(self, training_data):
        # پیاده‌سازی آموزش مدل
        self.model.fit(training_data)
        
    def predict(self, input_data):
        # پیاده‌سازی پیش‌بینی
        return self.model.predict(input_data)
        
    def generate_payload(self, context):
        # تولید پیلود مبتنی بر context
        return self.model.generate(context)

# ثبت مدل در فریمورک
framework.register_ai_model("my_model", MyCustomModel())
```

2. اضافه کردن اسکنر آسیب‌پذیری جدید / Adding New Vulnerability Scanner

```python
from framework import VulnerabilityScanner

class XXSScanner(VulnerabilityScanner):
    def scan(self, target_url, parameters):
        # پیاده‌سازی منطق اسکن XSS
        results = []
        for param in parameters:
            payload = self.generate_xss_payload()
            is_vulnerable = self.test_xss(target_url, param, payload)
            if is_vulnerable:
                results.append({
                    'vulnerable': True,
                    'parameter': param,
                    'payload': payload
                })
        return results
    
    def validate_finding(self, response, payload):
        # اعتبارسنجی یافته XSS
        return payload in response.text

# ثبت اسکنر در فریمورک
framework.register_scanner("xss", XXSScanner())
```

3. اتصال به API داده آموزشی / Connecting to Training Data API

```python
from framework import TrainingDataAPI

class MyTrainingAPI(TrainingDataAPI):
    def __init__(self, api_key, base_url):
        super().__init__()
        self.api_key = api_key
        self.base_url = base_url
        
    def fetch_training_data(self, data_type="all"):
        # دریافت داده از API شخصی
        headers = {"Authorization": f"Bearer {self.api_key}"}
        response = requests.get(
            f"{self.base_url}/training-data/{data_type}",
            headers=headers
        )
        return response.json()

# ثبت API در فریمورک
api = MyTrainingAPI("your-api-key", "https://api.example.com")
framework.register_data_api("my_api", api)
```

📚 API Documentation

VulnerabilityScannerFramework Class

متدهای اصلی / Main Methods

```python
class VulnerabilityScannerFramework:
    def register_ai_model(self, name: str, model_instance: AIModelInterface):
        """ثبت مدل AI جدید / Register new AI model"""
        
    def register_scanner(self, vuln_type: str, scanner_instance: VulnerabilityScanner):
        """ثبت اسکنر جدید / Register new scanner"""
        
    def register_data_api(self, name: str, api_instance: TrainingDataAPI):
        """ثبت API داده جدید / Register new data API"""
        
    def scan_target(self, target_url: str, scan_types: list = None) -> list:
        """اسکن هدف برای آسیب‌پذیری‌ها / Scan target for vulnerabilities"""
        
    def train_models(self, training_data: dict = None):
        """آموزش تمام مدل‌های ثبت شده / Train all registered models"""
```

AIModelInterface

```python
class AIModelInterface(ABC):
    @abstractmethod
    def load_model(self, model_path=None):
        """بارگذاری مدل / Load model"""
        
    @abstractmethod
    def train(self, training_data):
        """آموزش مدل / Train model"""
        
    @abstractmethod
    def predict(self, input_data):
        """پیش‌بینی / Make prediction"""
        
    @abstractmethod
    def generate_payload(self, context):
        """تولید پیلود / Generate payload"""
```

🛠 مثال‌های توسعه / Development Examples

مثال 1: مدل KNN سفارشی / Custom KNN Model

```python
from sklearn.neighbors import KNeighborsClassifier
from framework import MLModel

class KNNVulnerabilityModel(MLModel):
    def __init__(self, n_neighbors=5):
        super().__init__()
        self.n_neighbors = n_neighbors
        
    def load_model(self, model_path=None):
        if model_path and os.path.exists(model_path):
            self.model = joblib.load(model_path)
        else:
            self.model = KNeighborsClassifier(n_neighbors=self.n_neighbors)
            
    def train(self, training_data):
        X = [self.extract_features(item) for item in training_data['samples']]
        y = training_data['labels']
        self.model.fit(X, y)
        self.is_trained = True
        
    def predict(self, input_data):
        features = self.extract_features(input_data)
        return self.model.predict([features])[0]
```

مثال 2: اسکنر LFI جدید / New LFI Scanner

```python
from framework import VulnerabilityScanner

class LFIScanner(VulnerabilityScanner):
    def scan(self, target_url, parameters):
        findings = []
        lfi_payloads = [
            "../../etc/passwd",
            "....//....//etc/passwd",
            "../../windows/win.ini"
        ]
        
        for param in parameters:
            for payload in lfi_payloads:
                test_url = self.inject_payload(target_url, param, payload)
                response = self.http_client.robust_request(test_url)
                
                if self.is_lfi_vulnerable(response, payload):
                    findings.append({
                        'vulnerable': True,
                        'parameter': param,
                        'payload': payload,
                        'evidence': 'File content found in response'
                    })
                    
        return findings
```

مثال 3: API داده از گیت‌هاب / GitHub Data API

```python
class GitHubTrainingAPI(TrainingDataAPI):
    def fetch_training_data(self, data_type="all"):
        url = f"https://api.github.com/repos/payloadbox/{data_type}-payloads/contents"
        response = requests.get(url)
        
        if response.status_code == 200:
            files = response.json()
            payloads = []
            
            for file in files:
                if file['name'].endswith('.txt'):
                    content_url = file['download_url']
                    content = requests.get(content_url).text
                    payloads.extend(content.splitlines())
                    
            return payloads
        return []
```
