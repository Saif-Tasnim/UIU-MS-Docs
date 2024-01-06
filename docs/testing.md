# Unit Testing

There is provided testing unit on some cases for improving better result of uiu ms project.

## Login Test

### Description

Test the login functionality using Selenium WebDriver. This feature is tested by Saif Tasnim Chowdhury

### Code

```javascript
def test_login():
  it('log in as a student', async () => {
  await driver.get('http://localhost:5173');
  await driver.findElement(By.id('email')).sendKeys('schowdhury201223@bscse.uiu.ac.bd');
  await driver.findElement(By.id('password')).sendKeys('123456', Key.RETURN);
  const dashboardTitle = await driver.getTitle();
  assert.strictEqual(dashboardTitle, 'Student Dashboard');
});
```

## Counselling Request Test

### Description

Test the process of sending a counselling request using Selenium WebDriver. This features is tested by Arafat Hossen

### Code

```javascript
it("send a counselling request", async () => {
  await driver.get("http://localhost:5173");
  await driver.findElement(By.id("counselingButton")).click();
  const requestSuccessMessage = await driver
    .findElement(By.id("requestMessage"))
    .getText();
  assert.strictEqual(
    requestSuccessMessage,
    "Counseling request sent successfully."
  );
});
```

## Enroll Course Test

### Description

Test the course enrollment process using Selenium WebDriver. This features is tested by Abdul Muhit Chowdhury

### Code

```javascript
it("enroll a student into a course", async () => {
  await driver.get("http://localhost:5173");
  await driver.findElement(By.id("enrollButton")).click();
  const enrollmentSuccessMessage = await driver
    .findElement(By.id("enrollmentMessage"))
    .getText();
  assert.strictEqual(
    enrollmentSuccessMessage,
    "Successfully enrolled to the course."
  );
});
```

## Post Blog Test

### Description

Test the functionality of posting a blog using Selenium WebDriver. This features is tested by Iftakharul Islam Ifty

### Code

```javascript
it("allow a student to post a blog", async () => {
  await driver.get("http://localhost:5173");
  await driver.findElement(By.id("blogButton")).click();
  await driver
    .findElement(By.id("blogContent"))
    .sendKeys("Sample blog content...");
  await driver.findElement(By.id("postButton")).click();
  const postedBlog = await driver.findElement(By.id("latestBlog")).getText();
  assert.strictEqual(postedBlog, "Sample blog content...");
});
```

## Counselling Acceptance Test

### Description

Test the process of accepting counselling requests using Selenium WebDriver. This features is tested by Sirajum Monira Soha

### Code

```javascript
it("send a counselling request", async () => {
  await driver.get("http://localhost:5173");
  await driver.findElement(By.id("counselingButton")).click();
  const requestSuccessMessage = await driver
    .findElement(By.id("requestMessage"))
    .getText();
  assert.strictEqual(requestSuccessMessage, "Counseling request accepted.");
});
```
