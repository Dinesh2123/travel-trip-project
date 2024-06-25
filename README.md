# Travel Trip

This project is an individual assessment to build a **Travel Trip** app using React. The app will fetch data from an internal server, utilize routing concepts, handle authentication and authorization, and ensure responsiveness.

## Prerequisites

### UI Prerequisites

<details>
<summary>Click to view</summary>

- **Figma**: A vector graphics editor and prototyping tool. More info [here](https://www.figma.com/).
- **Create a Free Figma Account**: Follow the instructions in [this video](https://www.youtube.com/watch?v=hrHL2VLMl7g&t=37s) up to 00:50.
- **Check CSS in Figma**: Follow the instructions in [this video](https://www.youtube.com/watch?v=B242nuM3y2s) up to 02:45.
- **Export Images in Figma**: Follow the instructions in [this video](https://www.youtube.com/watch?v=NpzL1MONwaw).
- **Upload Images to Cloudinary**: Follow the session [here](https://www.figma.com/file/XoGFET0MdppCNgH6RhvcQe/Mini-Project---Travel-Trip?type=design&node-id=0-3523&mode=design&t=S89jMW84CTwn2Mkc-11) for better understanding.

</details>

### Design Files

<details>
<summary>Click to view</summary>

- Check the **Design Files** for different devices [here](https://www.figma.com/file/XoGFET0MdppCNgH6RhvcQe/Mini-Project---Travel-Trip?type=design&node-id=0-3523&mode=design&t=S89jMW84CTwn2Mkc-11).

</details>

## Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running:
  ```bash
  npm install
  ```
- Start the app using:
  ```bash
  npm start
  ```
</details>

## Completion Instructions

<details>
<summary>Functionality to be added</summary>
<br/>

### Login Route

- Display error message for invalid credentials.
- Navigate to Home Route on valid credentials.
- Redirect unauthenticated users to Login Route when accessing Home, Book A New Trip, or My Trips Routes.
- Redirect authenticated users to Home, Book A New Trip, or My Trips Routes.
- Redirect authenticated users from Login Route to Home Route.
- Toggle password visibility using the eye icon.

### Home Route

- Navigate to Book A New Trip Route on clicking **Book A New Trip** button.

### Book A New Trip Route

- Display **Your Details** form with Name, Start Location, End Location, and Next button.
  - Show respective error messages for empty fields.
  - Persist input values and navigate between steps.
  - Validate dates and display **Date Selection** form.
  - Handle **Guests** selection.
  - Provide **Travel Assistance** options.
  - Display **Confirmation** form with all details.
  - Allow cancelling or confirming the trip booking.

### My Trips Route

- Display trip details in cards.
- Show **No trips** screen if no trips are created.

### Header

- Navigate to Home Route on clicking website logo.
- Navigate to Home or My Trips Routes on clicking respective links.
- Navigate to Login Route on clicking Logout button.

- Ensure responsive design for mobile and tablet views.

</details>

<details>
<summary>API Requests & Responses</summary>
<br/>

**Login API**

- **URL**: `https://apis.ccbp.in/login`
- **Method**: `POST`
- **Request**:
  ```json
  {
    "username": "rahul",
    "password": "rahul@2021"
  }
  ```
- **Success Response**:
  ```json
  {
    "jwt_token": "sample_jwt_token"
  }
  ```
- **Failure Response**:
  ```json
  {
    "status_code": 404,
    "error_msg": "Username is not found"
  }
  ```

</details>

## Important Note

<details>
<summary>Click to view</summary>

- **HTML Elements for Styling**: Use HTML elements to style React Components. Usage of `styled-components` is not supported.
- **data-testid**: Use `data-testid` attribute in HTML elements.
  - Example: `<div data-testid="questionItem" className="question-item"/>`

- **Routes**:
  - `Home` Route: `/`
  - `My Trips` Route: `/my-trips`
  - `Book A New Trip` Route: `/book-a-new-trip`

- **Header**:
  - Travel Trip Logo font-family: `Caveat`

- **Login Route**:
  - Logo font-family: `Caveat`
  - Show password eye icon: `data-testid="show-password"`

- **Book A New Trip Route**:
  - Completed image alt attribute: value of `displayText` key from initial steps list.
  - Confirmed message image alt attribute: `success`.

- **Not Found Route**:
  - Not Found image alt attribute: `not found`

- Follow the screens as shown in the Figma design.

</details>

## Resources

<details>
<summary>Image URLs</summary>

- [Success Image](https://assets.ccbp.in/frontend/react-js/travel-trip-steps-successfully-completed-img.png)

</details>

<details>
<summary>Colors</summary>

**Background Colors**:
- ![#3b82f6](https://placehold.co/15x15/3b82f6/3b82f6.png) `#3b82f6`
- ![#304766](https://placehold.co/15x15/304766/304766.png) `#304766`
- ![#ffffff](https://placehold.co/15x15/ffffff/ffffff.png) `#ffffff`
- ![#2563eb](https://placehold.co/15x15/2563eb/2563eb.png) `#2563eb`
- ![#dbeafe](https://placehold.co/15x15/dbeafe/dbeafe.png) `#dbeafe`

**Text Colors**:
- ![#334155](https://placehold.co/15x15/334155/334155.png) `#334155`
- ![#2563eb](https://placehold.co/15x15/2563eb/2563eb.png) `#2563eb`
- ![#1e293b](https://placehold.co/15x15/1e293b/1e293b.png) `#1e293b`
- ![#ffffff](https://placehold.co/15x15/ffffff/ffffff.png) `#ffffff`
- ![#64748b](https://placehold.co/15x15/64748b/64748b.png) `#64748b`
- ![#f1f5f9](https://placehold.co/15x15/f1f5f9/f1f5f9.png) `#f1f5f9`
- ![#475569](https://placehold.co/15x15/475569/475569.png) `#475569`

**Border Colors**:
- ![#cbd5e1](https://placehold.co/15x15/cbd5e1/cbd5e1.png) `#cbd5e1`
- ![#e2e8f0](https://placehold.co/15x15/e2e8f0/e2e8f0.png) `#e2e8f0`

</details>

<details>
<summary>Font-families</summary>

- **Caveat**
- **Roboto**

</details>

## Project Submission Instructions

- Submit test cases at your own pace. The completion percentage will be considered for interviews.
- Publish your code frequently.

### _Things to Keep in Mind_

- All components should go in the `src/components` directory.
- **Do not remove pre-filled code**.
- Review the Cheat Sheets for quick references on concepts.

---
