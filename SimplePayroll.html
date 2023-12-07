<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Payroll Management</title>

    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #3498db; /* Blue background */
            text-align: center;
            color: white; /* White text */
            margin: 50px;
        }

        h2 {
            color: #fff; /* White text */
        }

        label {
            font-size: 16px;
            margin-right: 10px;
            color: #fff; /* White text */
            display: inline-block;
            text-align: left;
            width: 150px; /* Adjust the width as needed */
        }

        input, button {
            padding: 10px;
            font-size: 16px;
            border: 1px solid #fff; /* White border */
            border-radius: 5px;
            background-color: #fff; /* White background */
            color: #3498db; /* Blue text */
            margin-bottom: 10px;
            display: inline-block;
        }

        button {
            cursor: pointer;
        }

        button:hover {
            background-color: #2980b9; /* Slightly darker blue on hover */
        }

        #payrollTable {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }

        #payrollTable th, #payrollTable td {
            padding: 10px;
            border: 1px solid #fff; /* White border */
        }

        #payrollTable th {
            background-color: #2980b9; /* Darker blue for header */
        }

        #payrollTable td {
            background-color: #fff; /* White background */
            color: #3498db; /* Blue text */
        }

        /* Pop-up Box Styles */
        .popup-container {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: #fff; /* White background */
            border: 1px solid #3498db; /* Blue border */
            border-radius: 5px;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
            z-index: 1;
        }

        .popup-container p {
            margin-bottom: 20px;
            color: #3498db; /* Blue text */
        }

        .popup-container button {
            padding: 10px;
            font-size: 16px;
            margin: 0 10px;
            cursor: pointer;
            color: #fff; /* White text */
            background-color: #3498db; /* Blue background */
        }

        .popup-container button:hover {
            background-color: #2980b9; /* Slightly darker blue on hover */
        }

        .overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
        }
    </style>
</head>
<body>

    <h2>Payroll Management</h2>

    <label for="employeeName">Employee Name:</label>
    <input type="text" id="employeeName">

    <br>

    <label for="daysWorked">Days Worked:</label>
    <input type="number" id="daysWorked">

    <br>

    <label for="dailyRate">Daily Rate:</label>
    <input type="number" id="dailyRate">

    <br>

    <label for="deductionAmount">Deduction Amount:</label>
    <input type="number" id="deductionAmount">

    <br>

    <button onclick="addEmployee()">Add Employee</button>

    <table id="payrollTable">
        <thead>
            <tr>
                <th>No.</th>
                <th>Employee Name</th>
                <th>Days Worked</th>
                <th>Daily Rate</th>
                <th>Gross Pay</th>
                <th>Deduction Amount</th>
                <th>Net Pay</th>
                <th>Action</th>
            </tr>
        </thead>
        <tbody id="payrollBody">
            <!-- Payroll details will be displayed here dynamically -->
        </tbody>
    </table>

    <br>

    <label for="deleteLineNumber">Enter Line Number to Delete:</label>
    <input type="number" id="deleteLineNumber" min="1">
    <button onclick="confirmDeleteEmployee()">Delete Employee</button>

    <!-- Pop-up Box -->
    <div class="overlay" id="overlay"></div>
    <div class="popup-container" id="popupContainer">
        <p>Do you want to delete this employee?</p>
        <button onclick="deleteEmployee()">Confirm</button>
        <button onclick="cancelDelete()">Cancel</button>
    </div>

    <script>
        let payrollList = [];

        function addEmployee() {
            const employeeName = document.getElementById('employeeName').value;
            const daysWorked = parseFloat(document.getElementById('daysWorked').value);
            const dailyRate = parseFloat(document.getElementById('dailyRate').value);
            const deductionAmount = parseFloat(document.getElementById('deductionAmount').value);

            const grossPay = daysWorked * dailyRate;
            const netPay = grossPay - deductionAmount;

            const employee = {
                name: employeeName,
                daysWorked: daysWorked,
                dailyRate: dailyRate,
                grossPay: grossPay,
                deductionAmount: deductionAmount,
                netPay: netPay
            };

            payrollList.push(employee);
            displayPayrollList();
            clearInputFields();
        }

        function confirmDeleteEmployee() {
            document.getElementById('overlay').style.display = 'block';
            document.getElementById('popupContainer').style.display = 'block';
        }

        function deleteEmployee() {
            const deleteLineNumber = parseInt(document.getElementById('deleteLineNumber').value);
            if (deleteLineNumber >= 1 && deleteLineNumber <= payrollList.length) {
                payrollList.splice(deleteLineNumber - 1, 1);
                closePopup();
                displayPayrollList();
            } else {
                alert("Invalid line number. Please enter a valid line number.");
            }
        }

        function cancelDelete() {
            closePopup();
        }

        function closePopup() {
            document.getElementById('overlay').style.display = 'none';
            document.getElementById('popupContainer').style.display = 'none';
        }

        function displayPayrollList() {
            const payrollBody = document.getElementById('payrollBody');
            payrollBody.innerHTML = ''; // Clear existing content

            payrollList.forEach((employee, index) => {
                const row = document.createElement('tr');
                row.innerHTML = `
                    <td>${index + 1}</td>
                    <td>${employee.name}</td>
                    <td>${employee.daysWorked}</td>
                    <td>${employee.dailyRate}</td>
                    <td>${employee.grossPay}</td>
                    <td>${employee.deductionAmount}</td>
                    <td>${employee.netPay}</td>
                    <td><button onclick="confirmDeleteEmployee()">Delete</button></td>
                `;
                payrollBody.appendChild(row);
            });
        }

        function clearInputFields() {
            document.getElementById('employeeName').value = '';
            document.getElementById('daysWorked').value = '';
            document.getElementById('dailyRate').value = '';
            document.getElementById('deductionAmount').value = '';
        }
    </script>

</body>
</html>
