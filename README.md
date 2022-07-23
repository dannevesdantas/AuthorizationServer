# AuthorizationServer

The following steps show how to test your OAuth implementation to ensure that it works correctly:
1. Open the example project in Visual Studio and press F5 to run the project.
2. A new web browser window should open with your web application. Click the Register link located on the top-left corner of the page.
3. On the Register page, add an email address and password and confirm the password. Then click the Register button. You are going to use this user to grant privileges to the OAuth client for making requests to the /OAuth/Me endpoint.
4. Once you have registered the new user, you are automatically logged on and redirected to the Home page.
5. On the Home page, click your user’s email link at the top-left corner of the Home page.
6. On the Manage page, click the Authorize button, which redirects you to the Authorization Server page.
7. On the Authorization Server page, review the information provided and click the Grant button. After you grant access to the OAuth client application, you get the access and refresh token shown in Figure 3-3, which is needed to make requests to the resource server.
8. Click the Access Protected Resource API to make a request to the /OAuth/Me endpoint. You should get all information stored in the identity claim that you use for making this request, including the scopes bio and notes.
