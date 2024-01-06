# API Reference

### Course Enrollment

#### GET Method: 
this request is done by Saif Tasnim Chowdhury

```javascript
$.ajax({
  url: '/login',
  method: 'GET',
  
  success: function(response) {
    console.log(response);
  },
  error: function(error) {
    console.error(error);
  }
});
```

### Course Enrollment

#### Post Method: 
this request is done by Saif Tasnim Chowdhury

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

#### Post Method:
this request is done by Arafat Hossen

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

#### Post Method:
this request is done by Abdul Muhit Chowdhury

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

#### Post Method:
this request is done by Iftakharul Islam Ifty

```javascript
$.ajax({
  url: '/shuttle-schedule',
  method: 'POST',
   data: {
    up_time: 'Shuttle_Up_Time',
    shuttle_no: 'Shuttle_No',
    from: 'Shuttle_From',
    to : "Shuttle_to",
    current: "Shuttle_Current_Location"
    staffId: 'STAFF_ID',
  },
  success: function(response) {
    console.log(response);
  },
  error: function(error) {
    console.error(error);
  }
});
```

### Issue Sending Admin

#### Post Method:
this request is done by Sirajum Monira Soha

```javascript
$.ajax({
  url: '/issue-complaining',
  method: 'POST',
  data: {
    subject: 'Issue_Subject',
    desc: 'Issue_Description',
    staffId: 'STAFF_ID',
  },
  success: function(response) {
    console.log(response);
  },
  error: function(error) {
    console.error(error);
  }
});
```


