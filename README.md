## React Lab: Fetching and Rendering Data with Custom Hooks

##  Overview
In this lab, I created a React component named **`FetchData`** responsible for rendering fetched data onto the user interface. It uses a **custom hook** called **`useFetch`** to retrieve data from an API endpoint specified by a URL. The project demonstrates modular design in React by separating fetching logic from UI rendering, improving code readability and reusability.

---

## Components and Functionality
###  FetchData Component
- The **`FetchData`** component handles rendering of fetched data.
- It calls the **`useFetch`** hook to retrieve data asynchronously from the provided API URL.
- It uses the **`.map()`** method to iterate over the fetched data array and render each item dynamically within JSX elements.
- Each list item displays key details such as:
  - **Name**
  - **Importance**
  - **Benefits**
  - **Best Time to Intake**
- The data is displayed using styled list elements for a clean and readable UI.

### useFetch Custom Hook
- The **`useFetch`** hook encapsulates all the logic for fetching data from a given endpoint.
- Internally, it uses **`useState`** and **`useEffect`** to:
  - Fetch data asynchronously.
  - Store the results in state.
  - Handle loading and error states efficiently.
- By passing any API URL to this hook, multiple components can reuse the same fetching logic, making the code modular and scalable.

**Example usage:**
```jsx
const { data, loading, error } = useFetch('https://api.example.com/data');
```

### From this lab, I have learned to:

- Build and use custom React hooks for reusable logic.

- Implement asynchronous data fetching with useEffect.

- Manage state effectively using useState.

- Render lists dynamically with .map() and JSX.

- Apply modular design principles for scalability and clarity.