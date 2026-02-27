# Online Math Class Video Platform Plan

## Goal
Build a simple website/app where a math teacher uploads recorded classes and students can log in, watch lessons, and track what they have completed.

## Recommended MVP (first version)
1. **Teacher uploads videos**
   - Upload MP4 class recordings.
   - Add title, class level (e.g., Grade 10), chapter, and lesson number.
2. **Student accounts**
   - Students sign in with email/password.
   - Students only see classes assigned to their grade/batch.
3. **Course library**
   - Videos grouped by chapter and topic.
   - Search and filter by chapter.
4. **Video player with progress**
   - Save watch progress.
   - Mark lesson as completed.
5. **Basic dashboard**
   - Teacher sees number of students and lesson completion percentages.

## Tech options

### Option A: Fast no-code/low-code launch (quickest)
- Use **Google Drive + YouTube Unlisted + Google Classroom** (very fast).
- Pros: low cost, easy setup.
- Cons: limited control and branding.

### Option B: Custom web app (recommended for growth)
- Frontend: React / Next.js
- Backend: Node.js / NestJS or Django
- Database: PostgreSQL
- Video storage/streaming: AWS S3 + CloudFront or Vimeo API
- Auth: Firebase Auth / Auth0 / custom JWT

## Suggested database entities
- `users` (teacher, student)
- `courses`
- `lessons`
- `videos`
- `enrollments`
- `lesson_progress`

## Must-have features after MVP
- Live class links (Zoom/Meet integration)
- Notes and downloadable PDFs
- Doubt/Question section per lesson
- Quizzes after each chapter
- Mobile app (Android first)

## Security and privacy basics
- Private videos (not public links)
- Role-based access (teacher/student/admin)
- HTTPS and encrypted passwords
- Backup strategy for uploaded content

## Rollout plan
1. Week 1: Requirements + UI wireframes
2. Week 2-3: Authentication, upload, lesson listing
3. Week 4: Video player + progress tracking
4. Week 5: Teacher dashboard + testing
5. Week 6: Pilot with one class and collect feedback

## Practical recommendation for your teacher
Start with an MVP that only includes:
- Teacher upload
- Student login
- Chapter-wise video library
- Progress tracking

Then grow based on student feedback.
