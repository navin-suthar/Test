# React Data Table App

## Task
Create a React app that fetches data from the following API and displays it in a data table with pagination and sorting. Additionally, include search functionality in the table.

API: [https://jsonplaceholder.typicode.com/posts](https://jsonplaceholder.typicode.com/posts)

## Solution
The solution involves creating a `DataTable` component that handles data fetching, sorting, filtering, and pagination. The functionalities are implemented as follows:

### 1. Data Fetching
Data is fetched from the API using the `fetch` method within the `useEffect` hook. The fetched data is stored in the component's state.

### 2. Sorting
Sorting functionality is implemented by modifying the `handleSort` function and the `sortedData` function. The `handleSort` function toggles the sort direction and updates the `sortConfig` state, which is used to sort the data accordingly.

### 3. Filtering
Filtering is implemented using an input field that updates the `searchTerm` state. The filtering logic is applied to the sorted data to ensure the displayed results are both sorted and filtered based on the search term.

### 4. Pagination
Pagination logic is implemented to calculate the current rows based on the filtered and sorted data. The pagination controls allow navigation between pages, and the number of rows per page can be adjusted. The current page is reset to 1 when searching or changing the number of rows per page.
