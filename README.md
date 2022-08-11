# address-book-app
This is a simple app which has a databse that stores contact information of various users. The front end interface is made using React with Ant Design components. Ant design components handle much of redundancy of creating UI elements and has built in functionality.

## Approach.
All of the data management is handled by the custom hook useData, this custom hook either updates the Data Storage reducer on the API call to update all the cards, or appends content at the end until 1000 results have been displayed.
The settings and homepage are handled by react router, where the switch handles switching between elements. In the settings page, the form uodates the settings reducer, a useEffect hook updates the main page whenever settings are updated. And before calling the API, it checks the nationality and gender parameters from the settings Reducer.
The modal is called whenever any card is clicked. Before loading the modal, the index of the item clicked is stored in the reducer, when the modal is displayed, data stored at the index is passed as props, and then displayed in the modal. The modal is styled voa LESS using flexbox design.
