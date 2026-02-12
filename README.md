# Chore--Scheduler
a simple chore scheduling for house mates
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chore Scheduler</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <header>
            <h1>🏠 Chore Scheduler</h1>
            <p>Keep your home clean and organized!</p>
        </header>

        <main>
            <!-- Add Chore Form -->
            <section class="form-section">
                <h2>Add a New Chore</h2>
                <form id="choreForm">
                    <div class="form-group">
                        <label for="choreName">Chore Name:</label>
                        <input type="text" id="choreName" placeholder="e.g., Vacuum, Dishes, Bathroom" required>
                    </div>

                    <div class="form-group">
                        <label for="assignee">Assign to:</label>
                        <input type="text" id="assignee" placeholder="Housemate name" required>
                    </div>

                    <div class="form-group">
                        <label for="dueDate">Due Date:</label>
                        <input type="date" id="dueDate" required>
                    </div>

                    <div class="form-group">
                        <label for="priority">Priority:</label>
                        <select id="priority">
                            <option value="low">Low</option>
                            <option value="medium" selected>Medium</option>
                            <option value="high">High</option>
                        </select>
                    </div>

                    <button type="submit" class="btn btn-primary">Add Chore</button>
                </form>
            </section>

            <!-- Schedule View -->
            <section class="schedule-section">
                <h2>📅 Chore Schedule</h2>
                <div id="choreList" class="chore-list">
                    <p class="empty-message">No chores yet. Add one above!</p>
                </div>
            </section>
        </main>

        <footer>
            <p>Made with ❤️ for a clean home</p>
        </footer>
    </div>

    <script src="script.js"></script>
</body>
</html>
