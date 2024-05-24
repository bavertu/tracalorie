# Tracalorie 2.0
https://tracalorie-pied.vercel.app
## Overview
Tracalorie 2.0 is a web application designed to help users track their daily caloric intake and expenditure. It allows users to set a daily calorie limit, add meals and workouts, and see the balance between calories consumed and burned. The application stores data locally using the browser's localStorage.

## Features
- **Set Daily Calorie Limit**: Users can set their daily calorie limit through a modal form.
- **Track Calories Consumed and Burned**: Add meals and workouts to track calories consumed and burned.
- **Display Caloric Statistics**: View daily statistics including total calories consumed, burned, and remaining.
- **Filter Items**: Filter meals and workouts for easy management.
- **Reset Data**: Reset daily data to start fresh.

## Installation
To run the application locally:

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/tracalorie.git
    cd tracalorie
    ```

2. Install dependencies (if any):
    ```sh
    npm install
    ```

3. Open `index.html` in your preferred web browser:
    ```sh
    open index.html
    ```

## Usage

### Setting Calorie Limit
1. Click the "Set Daily Limit" button.
2. Enter your desired daily calorie limit in the modal that appears.
3. Click "Save" to set the limit.

### Adding Meals
1. Click the "Add Meal" button under the "Meals / Food Items" section.
2. Enter the meal name and the number of calories.
3. Click "Add Meal Item" to save.

### Adding Workouts
1. Click the "Add Workout" button under the "Workouts" section.
2. Enter the workout name and the number of calories burned.
3. Click "Add Workout Item" to save.

### Filtering Items
1. Use the "Filter Meals..." or "Filter Workouts..." input fields to filter items by name.

### Resetting Data
1. Click the "Reset Day" button to clear all data for the day.

## Classes

### `Meal`
- **Properties**:
  - `id`: Unique identifier for the meal.
  - `name`: Name of the meal.
  - `calories`: Number of calories in the meal.

### `Workout`
- **Properties**:
  - `id`: Unique identifier for the workout.
  - `name`: Name of the workout.
  - `calories`: Number of calories burned in the workout.

### `Storage`
- **Methods**:
  - `getCalorieLimit()`: Retrieves the calorie limit from localStorage.
  - `setCalorieLimit(limit)`: Sets the calorie limit in localStorage.
  - `getTotalCalories()`: Retrieves the total calories from localStorage.
  - `updateTotalCalories(calories)`: Updates the total calories in localStorage.
  - `getMeals()`: Retrieves the meals from localStorage.
  - `saveMeal(meal)`: Saves a meal to localStorage.
  - `removeMeal(id)`: Removes a meal from localStorage.
  - `getWorkouts()`: Retrieves the workouts from localStorage.
  - `saveWorkout(workout)`: Saves a workout to localStorage.
  - `removeWorkout(id)`: Removes a workout from localStorage.
  - `clearAll()`: Clears all data from localStorage.

### `CalorieTracker`
- **Methods**:
  - `addMeal(meal)`: Adds a meal and updates total calories.
  - `addWorkout(workout)`: Adds a workout and updates total calories.
  - `removeMeal(id)`: Removes a meal and updates total calories.
  - `removeWorkout(id)`: Removes a workout and updates total calories.
  - `reset()`: Resets all data.
  - `setLimit(calorieLimit)`: Sets a new calorie limit.
  - `loadItems()`: Loads meals and workouts from localStorage.

## External Libraries
- [Font Awesome](https://fontawesome.com/): Icons
- [Bootstrap](https://getbootstrap.com/): CSS framework

## Contributing
To contribute to this project, fork the repository, create a new branch, and submit a pull request. Please ensure all new code is well-documented and tested.

## License
This project is licensed under the MIT License.

---

Feel free to customize this `README.md` file to better fit your specific needs. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.
