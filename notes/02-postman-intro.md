# 🔰 **Postman Introduction Tutorial**

## 🧠 What is Postman?

**Postman** is a popular API client used for developing, testing, and documenting APIs. It provides a graphical user interface to send HTTP requests and view responses.

### ✅ **Why Use Postman?**

- No need to write code to test APIs
- User-friendly interface
- Supports all HTTP methods (GET, POST, PUT, DELETE, etc.)
- Helps in debugging APIs
- Supports automation using **Collections** and **Environments**
- Can be used for **Manual** as well as **Automated** testing

---

## 🔧 **Installing Postman**

### 🖥️ Desktop Version

1. Visit [https://www.postman.com/downloads](https://www.postman.com/downloads)
2. Download and install the Postman App for Windows/Mac/Linux

### 🌐 Web Version (No installation)

- Visit: [https://web.postman.co](https://web.postman.co)
- Login using your email or Google account

---

## 📦 **Understanding Basic Components of Postman**

| Component       | Description                                                  |
| --------------- | ------------------------------------------------------------ |
| **Request**     | The API call made to a server (GET, POST, etc.)              |
| **Response**    | The server's reply to the request                            |
| **Collection**  | A folder to organize saved API requests                      |
| **Environment** | Set of variables (like base URL, API key) that can be reused |
| **History**     | Automatically stores previously sent requests                |

---

## ▶️ **Making Your First API Request**

### Example: Send a `GET` request to a public API

1. Open Postman
2. In the top-left corner, click `+` to open a new tab
3. Set the method to `GET`
4. Enter this URL:

   ```
   https://jsonplaceholder.typicode.com/posts/1
   ```

5. Click on the blue **Send** button
6. Check the **response** in the bottom pane

---

## 💬 **HTTP Methods in Postman**

| Method   | Description         | Example                    |
| -------- | ------------------- | -------------------------- |
| `GET`    | Retrieve data       | `Get list of users`        |
| `POST`   | Create data         | `Add new user`             |
| `PUT`    | Update data         | `Update entire record`     |
| `PATCH`  | Update partial data | `Update user's email only` |
| `DELETE` | Remove data         | `Delete a user`            |

---

## 🧪 **Create a POST Request**

### Step-by-Step:

1. Select `POST` as the method
2. URL:

   ```
   https://jsonplaceholder.typicode.com/posts
   ```

3. Click on **Body** tab → select **raw** → choose **JSON**
4. Enter JSON payload:

```json
{
  "title": "Postman Tutorial",
  "body": "This is a test post.",
  "userId": 1
}
```

5. Click **Send**
6. You will get a response with a newly created post ID

---

## 🧰 **Advanced Features (Overview)**

| Feature                | What It Does                                  |
| ---------------------- | --------------------------------------------- |
| **Collection**         | Save requests and share them                  |
| **Environment**        | Create variables for base URL, API keys, etc. |
| **Pre-request Script** | Run JS code before sending a request          |
| **Tests**              | Write test scripts to validate API response   |
| **Monitor**            | Run tests on schedule and get reports         |
| **Mock Server**        | Simulate API endpoints for testing            |

---

## 📘 **Useful Public APIs to Practice**

- [https://jsonplaceholder.typicode.com/](https://jsonplaceholder.typicode.com/)
- [https://reqres.in/](https://reqres.in/)
- [https://dummyjson.com/](https://dummyjson.com/)
