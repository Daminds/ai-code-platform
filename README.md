# ai-code-platform
Frontend (React/Vite)       Backend (FastAPI)        AI Services
┌───────────────┐           ┌───────────────┐        ┌───────────────┐
│ Monaco Editor │  <----->  │ FastAPI       │ <----> │ Ollama        │
│ File Tree     │           │ Endpoints     │        │ (local models)│
│ Model Select  │           │ File Manager  │        ├───────────────┤
│ Testing Panel │           │ Test Runner   │        │ OpenAI API    │
└───────────────┘           └───────────────┘        └──────────────


\
│
├── ai-code-platform\               # Main project folder
│   │
│   ├── backend\                    # FastAPI backend
│   │   ├── app\                    # Application code
│   │   │   ├── __init__.py
│   │   │   ├── main.py            # FastAPI application
│   │   │   ├── models.py          # Data models
│   │   │   ├── routes\            # API endpoints
│   │   │   │   ├── generate.py
│   │   │   │   ├── files.py
│   │   │   │   └── __init__.py
│   │   │   ├── services\          # Business logic
│   │   │   │   ├── ai_service.py
│   │   │   │   ├── file_service.py
│   │   │   │   └── __init__.py
│   │   │   └── utils\             # Utilities
│   │   │       ├── config.py
│   │   │       └── __init__.py
│   │   │
│   │   ├── tests\                  # Unit tests
│   │   ├── venv\                   # Python virtual environment
│   │   ├── requirements.txt        # Python dependencies
│   │   ├── start_backend.ps1       # Startup script
│   │   └── .env                    # Environment variables
│   │
│   └── frontend\                   # React/Vite frontend
│       ├── public\
│       ├── src\
│       │   ├── assets\             # Static assets
│       │   ├── components\         # React components
│       │   │   ├── Editor\
│       │   │   ├── FileTree\
│       │   │   └── Toolbar\
│       │   ├── hooks\              # Custom hooks
│       │   ├── services\           # API services
│       │   ├── App.tsx
│       │   ├── main.tsx
│       │   └── vite-env.d.ts
│       ├── package.json
│       ├── tsconfig.json
│       ├── vite.config.ts
│       └── start_frontend.ps1      # Startup script
│
├── models\                         # Local AI model storage (Ollama)
│   ├── codellama\
│   └── gpt-engineer\
│
├── workspace\                      # User code projects
│   ├── project1\
│   └── project2\
│
└── backups\                        # Automatic file backups
    ├── project1\
    └── project2\
