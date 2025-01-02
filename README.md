# research-assistant

## Project Structure
research-assistant/
├── app/
│   ├── __init__.py
│   ├── main.py                  # FastAPI application entry point
│   ├── config/
│   │   ├── __init__.py
│   │   └── settings.py          # Pydantic settings management
│   ├── api/
│   │   ├── __init__.py
│   │   ├── v1/
│   │   │   ├── __init__.py
│   │   │   ├── router.py        # API route definitions
│   │   │   └── endpoints/
│   │   │       ├── __init__.py
│   │   │       ├── newsletter.py
│   │   │       └── subscribers.py
│   ├── core/
│   │   ├── __init__.py
│   │   ├── security.py          # Authentication & authorization
│   │   └── logging.py          
│   ├── models/
│   │   ├── __init__.py
│   │   ├── newsletter.py        # Pydantic models
│   │   └── subscriber.py
│   ├── services/
│   │   ├── __init__.py
│   │   ├── newsletter.py
│   │   ├── paper_analyzer.py
│   │   └── email.py
│   ├── prompts/
│   │   ├── __init__.py
│   │   └── newsletter_prompts.py
│   └── utils/
│       ├── __init__.py
│       └── aws.py
├── tests/
│   ├── __init__.py
│   ├── conftest.py
│   ├── test_api/
│   └── test_services/
├── alembic/                     # Database migrations
│   ├── versions/
│   └── alembic.ini
├── docker/
│   ├── Dockerfile
│   └── docker-compose.yml
├── scripts/
│   ├── start.sh
│   └── test.sh
├── .env.example
├── requirements.txt
├── requirements-dev.txt
└── README.md