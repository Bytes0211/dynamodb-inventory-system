# DynamoDB Inventory Management System

An AWS DynamoDB project demonstrating advanced features including Global Secondary Indexes (GSI), Local Secondary Indexes (LSI), DynamoDB Streams, Transactions, Batch Operations, and Query Optimization.

## 🎯 Project Overview

This project implements a complete inventory management system using DynamoDB, showcasing real-world patterns and best practices for designing scalable NoSQL applications.

## ✨ Key Features

### Core DynamoDB Concepts

- **Single Table Design** - Multiple entity types in one table


### Application Features

- Product inventory tracking with variants
- Order management with multiple items
- Warehouse location tracking
- Low stock alerts via DynamoDB Streams
- Audit logging for all changes
- Batch import/export functionality
- Transaction-based order fulfillment

## 🏗️ Architecture

⌛ Architecture design in progroess

## 🚀 Getting Started

### Prerequisites

- Python 3.12+
- AWS Account
- AWS CLI configured
- boto3 library
- maybe others

### Installation

```bash
# Clone the repository
git clone <repository-url>
cd dynamodb-inventory-system

# Create virtual environment
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Running Locally with DynamoDB Local

```bash
# Start DynamoDB Local (Docker)
docker run -p 8000:8000 amazon/dynamodb-local

# Set local endpoint
export DYNAMODB_ENDPOINT_URL=http://localhost:8500

```

### Stream Processing

```python
from stream_processor import LowStockAlertProcessor

# Process DynamoDB Stream events
processor = LowStockAlertProcessor()
processor.process_stream_records(stream_records)
```

## 🗂️ Project Structure

⌛ Inprogress

## 🤝 Contributing

Contributions welcome! Please read the contributing guidelines first.

## 📝 License

MIT License - See LICENSE file for details

---

**Note**: This is an educational project demonstrating DynamoDB concepts. For production use, consider additional security, monitoring, and error handling.
