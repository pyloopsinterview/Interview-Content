# Interview Q&A - Python Backend & Data Engineer (Almas)

## 1. Can you walk me through your experience with required skills?

**Answer:** I have around 12 years of experience working with Python,
focusing on building scalable backend systems and data platforms. I use
async programming extensively with asyncio and FastAPI for
high-performance services. I've built API integrations with retry and
backoff strategies, designed ETL pipelines using Prefect, and worked
heavily with Snowflake and PostgreSQL. I also use Pydantic for
validation and pytest for testing to ensure high code quality.

------------------------------------------------------------------------

## 2. How do you handle multiple external API calls without blocking the event loop?

**Answer:** I use async HTTP clients like httpx and run multiple API
calls concurrently using asyncio.gather. This allows parallel execution
without blocking. I then process responses and store results using async
database drivers like async SQLAlchemy. This ensures the entire flow is
non-blocking.

------------------------------------------------------------------------

## 3. How do you handle flexible payloads in Pydantic v2?

**Answer:** I use Union types to support multiple input formats and
apply model validators to normalize inputs. This ensures consistent
internal structure. For responses, I define separate response models and
use FastAPI's response_model to expose only required fields.

------------------------------------------------------------------------

## 4. How do you implement incremental loads with idempotency in Snowflake?

**Answer:** I use a watermark strategy (like last_updated_timestamp) to
extract only new data. Data is first loaded into a staging table, then
merged into the target table using a MERGE statement. Deduplication is
handled using window functions, and watermark is updated only after
successful execution.

------------------------------------------------------------------------

## 5. How do you handle retries for unreliable external APIs?

**Answer:** I implement retries using exponential backoff with Tenacity.
I retry only on transient errors like 5XX. I also configure timeouts and
optionally use circuit breakers to prevent system overload. All calls
are async to avoid blocking.

------------------------------------------------------------------------

## 6. How do you test FastAPI endpoints with DB and orchestration dependencies?

**Answer:** I use pytest and FastAPI TestClient. I override DB
dependencies with test databases and mock external systems like Prefect.
Fixtures ensure isolation, and no real external calls are made, keeping
tests fast and reliable.

------------------------------------------------------------------------

## 7. How do you handle PST timezone work?

**Answer:** I'm fully comfortable working in PST and flexible with
schedule overlap requirements.

------------------------------------------------------------------------

## 8. Current Work Status?

**Answer:** I'm currently working with CHRISTUS Health through my own
corporation, and my project is active.

------------------------------------------------------------------------

## 9. Job Search Status?

**Answer:** I'm actively exploring opportunities but not in final offer
stages yet.

------------------------------------------------------------------------

## 10. Work Authorization?

**Answer:** I'm a Green Card holder and do not require sponsorship.
