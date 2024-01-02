# API Reference

## Endpoints

### Course Enrollment

#### Request

```javascript
$.ajax({
  url: '/enroll',
  method: 'POST',
  data: {
    courseId: 'COURSE_ID',
    userId: 'USER_ID',
  },
  success: function(response) {
    console.log(response);
  },
  error: function(error) {
    console.error(error);
  }
});
```

### Counseling Request

#### Request

```javascript
$.ajax({
  url: '/request-counseling',
  method: 'POST',
  data: {
    facultyId: 'FACULTY_ID',
    studentId: 'STUDENT_ID',
    requestedTime: 'TIME',
  },
  success: function(response) {
    console.log(response);
  },
  error: function(error) {
    console.error(error);
  }
});
```

### Blog Sharing

#### Request

```javascript
$.ajax({
  url: '/share-blog',
  method: 'POST',
  data: {
    title: 'BLOG_TITLE',
    content: 'BLOG_CONTENT',
    authorId: 'AUTHOR_ID',
  },
  success: function(response) {
    console.log(response);
  },
  error: function(error) {
    console.error(error);
  }
});
```

### Shuttle Schedule

#### Request

```javascript
$.ajax({
  url: '/shuttle-schedule',
  method: 'GET',
  success: function(response) {
    console.log(response);
  },
  error: function(error) {
    console.error(error);
  }
});
```


