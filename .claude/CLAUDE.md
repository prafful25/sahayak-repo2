# SAHAYAK DATA  CLAUDE CODE CONTEXTSERVICES 
# Read this file first. Update SECTION 4 after every API completion.

## SECTION 1: PROJECT IDENTITY
Project  : Sahayak Data  Indian Government Data APIs (Repo 2)Services 
Owner    : Prafful Garg, Meerut UP
Stack    : FastAPI + PostgreSQL + Redis + n8n + Razorpay
Build Env: GitHub Actions (ubuntu-latest, 16GB RAM)

## SECTION 2: CODING CONVENTIONS (MANDATORY)
Python   : 3.11+, type hints on ALL functions, PEP8
Routes   : GET only. No POST except /webhooks/razorpay
Cache TTL: 30 min default | 5 min for prices | 24 hr for static
Redis key: {container}:{api_name}:{params_hash}
DB tables: snake_case, prefix sahayak_{container}_{api_name}
Error fmt: {"status":"error","code":4xx,"message":"...","timestamp":"ISO8601"}
Response : {"status":"success","data":{...},"meta":{"source":"...","cached":true}}
Tests    : pytest, minimum 3 tests per endpoint
Commits  : "build: {api_name} completeCommits  : "build: {api_name} cCTCommits  : "buiFECommits  : "build: {api_name} cURCommits  : "build: {api_name} completeCommits stAPI   : Each container = one folder under /api/
Tests     : Mirror strTests     : Mirror strTests  IOTests     : Mirror strTests     : Mirror strTests  IOTests     : Mirror e on. Never block.
