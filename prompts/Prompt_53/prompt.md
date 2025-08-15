# Prompt 53: Database Migration & Seeding Setup

Create comprehensive database migration and seeding system for production deployment:

## 1. Database Migration System
Create /src/database/migrations/ folder with:
- 001_initial_schema.sql: Complete database schema creation
- 002_add_indexes.sql: Performance optimization indexes
- 003_add_triggers.sql: Automated timestamp updates
- 004_add_functions.sql: Helper functions and procedures
- 005_add_sample_data.sql: Initial data for testing

## 2. Migration Scripts
Create /src/database/migrate.ts:
- Automated migration runner
- Version tracking in database
- Rollback capabilities
- Migration status checking
- Environment-specific migrations

## 3. Sample Data Seeding
Create /src/database/seed.ts:
- Sample recipes for testing
- Default dietary preferences
- Common ingredients database
- Sample user profiles
- Test meal plans

## 4. Database Utilities
Create /src/database/utils.ts:
- Connection pooling setup
- Query optimization helpers
- Backup and restore functions
- Database health checks
- Performance monitoring

## 5. Environment Setup
Create database configuration for:
- Development environment
- Staging environment  
- Production environment
- Test environment
- Local development

## 6. Migration Commands
Add to package.json scripts:
- npm run db:migrate
- npm run db:seed
- npm run db:reset
- npm run db:backup
- npm run db:health

## ✅ Verify Success:
- [ ] Run migrations successfully
- [ ] Sample data loads correctly
- [ ] Database health check passes
- [ ] All tables and indexes created
- [ ] Backup/restore functions work
