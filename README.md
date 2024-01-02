<h1>Lesson 1 Notes</h1>

<table>
  <tr>
    <th>File: <code>Store.js</code></th>
  </tr>
  <tr>
    <td>
      Redux store is created and configured. This file contains fundamental structures such as the application's state and reducers used to update this state.
      Additionally, it includes the <code>&lt;Provider&gt;</code> component to provide the Redux store to the React application.
    </td>
  </tr>
  <tr>
    <th>File: <code>&lt;Provider /&gt;</code></th>
  </tr>
  <tr>
    <td>
      Provides the Redux store to the overall component tree of the React application. This enables all components throughout the application to access and use the Redux store.
      The <code>&lt;Provider&gt;</code> component is placed at the top level of the React application and takes the Redux store as a prop.
    </td>
  </tr>
  <tr>
    <th>Slice & Reducer:</th>
  </tr>
  <tr>
    <td>
      Represents a logical part of the Redux store responsible for updating the state. Created using the <code>createSlice</code> function in Redux Toolkit, Slices bring together actions that update the state and reducers that respond to these actions.
      Slices provide a more modular and compact way to organize reducers and actions, keeping reducers and action creators within a single structure for cleaner code.
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>Advantages of State Slices:</th>
  </tr>
  <tr>
    <td>
      <strong>Modularity:</strong><br>
      State Slices provide a modular structure by breaking down the application state into distinct parts. Each Slice represents a specific feature or component.
    </td>
  </tr>
  <tr>
    <td>
      <strong>Cleaner Reducers:</strong><br>
      Slices make reducer functions, responsible for updating the state, more organized and readable. Each Slice is only responsible for updating its own state.
    </td>
  </tr>
  <tr>
    <td>
      <strong>Automatic Action Creator Generation:</strong><br>
      Redux Toolkit automatically generates action creators for Slices, simplifying the process of creating and dispatching actions.
    </td>
  </tr>
  <tr>
    <td>
      <strong>Initial State Definition:</strong><br>
      State Slices provide an <code>initialState</code> property to define the initial state. This allows each Slice to determine its own starting state.
    </td>
  </tr>
  <tr>
    <td>
      <strong>Thunk Middleware Integration:</strong><br>
      Redux Toolkit includes the Redux Thunk middleware to manage asynchronous operations. Together with Slices, Thunk middleware enables the integration of async operations into the Redux store.
    </td>
  </tr>
  <tr>
    <td>
      <strong>Usage of Immer:</strong><br>
      Redux Toolkit utilizes the Immer library to make updating state easier. Immer enables easy and readable updates on immutable data structures.
    </td>
  </tr>
</table>
