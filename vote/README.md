## 🛠️ Build & Run Configuration

| Item               | Description                                |
|--------------------|--------------------------------------------|
| **Base**           | `python:2.7-alpine`                        |
| **Work Directory** | `/app`                                     |
| **Build Instruction** | `pip install -r requirement.txt`        |
| **Port**           | `80`                                       |
| **Launch Command** | `gunicorn app:app -b 0.0.0.0:80`           |



