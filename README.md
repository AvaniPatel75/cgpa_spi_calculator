# CGPA & SPI Calculator

A Dart package to calculate SPI, CGPA, GPA using multiple grading scales.

## Features
- SPI calculation
- CGPA calculation
- Multiple grading scales
- Semester-wise analytics

## Usage

```dart
final semester = Semester(
  name: 'Sem 1',
  courses: [
    Course(name: 'Math', code: 'M101', credits: 4, grade: 'A', gradePoint: 8),
  ],
);

final record = AcademicRecord(
  semesters: [semester],
  gradingScale: GradingScales.tenPoint,
);

print(record.calculateCGPA());
