# spring-mvc-app-with-security
Built a Spring MVC application that secures the page with a login form that is backed by a fixed list of users

## Inspiration:
- https://spring.io/guides/gs/securing-web
- https://github.com/spring-guides/gs-securing-web

## Demo:
Once the application starts up, you should see the home page, as the following image shows:
<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/e9cb290e-635a-4514-addd-6b9b02a08eba" alt="home page" style="border: 2px solid black;"></td>
  </tr>
</table>

When you click on the link, it attempts to take you to the greeting page at /greeting. However, because that page is secured and you have not yet logged in, it takes you to the login page, as the following image shows:
<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/b9990152-f9f1-4ec2-921e-171e5048c0bd" alt="login page" style="border: 2px solid black;"></td>
  </tr>
</table>

At the login page, sign in as the test user by entering the username and password as configured in `WebSecurityConfig.java`. Once you submit the login form, you are authenticated and then taken to the greeting page, as the following image shows:
<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/af94e2b3-7147-45f3-8cbe-0ae8c818de73" alt="greeting page" style="border: 2px solid black;"></td>
  </tr>
</table>
Note: I have configured the test user's username to `rishit`.

If you click on the Sign Out button, your authentication is revoked, and you are returned to the login page with a message indicating that you are logged out:
<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/99cb7d1c-b5be-423f-843e-8f1c5c7b2acf" alt="logged out" style="border: 2px solid black;"></td>
  </tr>
</table>
