# 📘 **Creating a Collection in Postman and Adding CRUD Requests**

---

## 🔰 What is a Collection in Postman?

A **Collection** in Postman is a group of related API requests that can be saved, organized, shared, and tested together. It is useful for:

* Grouping requests (e.g., all user-related APIs)
* Running requests in a sequence
* Reusing environments and variables
* Sharing with teams

---

## 📦 Step 1: Create a New Collection

1. Open Postman.
2. On the left sidebar, click **Collections** tab.
3. Click the **“+ New Collection”** button.
4. Give it a **name** (e.g., `User API CRUD`)
5. (Optional) Add a **description**.
6. Click **Create**.

---

## 🧪 Step 2: Add CRUD Requests to the Collection

We’ll use the **Dummy API** from `https://jsonplaceholder.typicode.com`.

---

### 🟢 **1. GET Request – Fetch a User**

1. Click the **`+`** tab to open a new request.
2. Set method to `GET`
3. URL:

   ```
   https://jsonplaceholder.typicode.com/users/1
   ```
4. Click **Send** to test.
5. Click **Save**:

   * Name it: `Get User`
   * Choose the collection: `User API CRUD`

✅ This request fetches a user with ID 1.

---

### 🟡 **2. POST Request – Create a User**

1. Click `+` to create a new request.
2. Set method to `POST`
3. URL:

   ```
   https://jsonplaceholder.typicode.com/users
   ```
4. Go to **Body → raw → JSON**
5. Enter:

```json
{
  "name": "John Doe",
  "email": "john@example.com"
}
```

6. Click **Send**
7. Click **Save**:

   * Name: `Create User`
   * Collection: `User API CRUD`

✅ This request simulates creating a new user.

---

### 🔵 **3. PUT Request – Update a User (Full Update)**

1. Create new request.
2. Method: `PUT`
3. URL:

   ```
   https://jsonplaceholder.typicode.com/users/1
   ```
4. Body → raw → JSON:

```json
{
  "name": "John Updated",
  "email": "john_updated@example.com"
}
```

5. Click **Send**
6. Save as `Update User (PUT)` under `User API CRUD`

✅ Replaces the full record of the user with ID 1.

---

### 🟣 **4. PATCH Request – Update Partial User Data**

1. Create request.
2. Method: `PATCH`
3. URL:

   ```
   https://jsonplaceholder.typicode.com/users/1
   ```
4. Body → raw → JSON:

```json
{
  "email": "john_patch@example.com"
}
```

5. Click **Send**
6. Save as `Update User (PATCH)`

✅ Only updates the email of the user.

---

### 🔴 **5. DELETE Request – Remove a User**

1. Create request.
2. Method: `DELETE`
3. URL:

   ```
   https://jsonplaceholder.typicode.com/users/1
   ```
4. Click **Send**
5. Save as `Delete User`

✅ Deletes the user with ID 1 (simulated).

---

## 📂 Final Collection Structure

```
User API CRUD (Collection)
├── Get User
├── Create User
├── Update User (PUT)
├── Update User (PATCH)
└── Delete User
```

---


## ✅ Summary

| CRUD Operation | HTTP Method | Postman Request |
| -------------- | ----------- | --------------- |
| Create         | POST        | `Create User`   |
| Read           | GET         | `Get User`      |
| Update         | PUT / PATCH | `Update User`   |
| Delete         | DELETE      | `Delete User`   |

