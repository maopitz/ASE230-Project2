# Project 1 — REST API Documentation

## Overview
This project implements a Student Course Management REST API system built with **PHP**, **MySQL**, and **JSON-based endpoints**.

Endpoints include:
- `/students` (GET, POST)
- `/students/{id}` (GET, PUT, DELETE)
- `/courses` (GET, POST)
- `/enrollments` (POST, DELETE)
- `/students/{id}/courses` (GET)

Authentication:
- Bearer token stored in `api_tokens` table
- Required for enrollment endpoints

This page covers:
- API design  
- System structure  
- Example requests and responses  
- Authentication workflow  
