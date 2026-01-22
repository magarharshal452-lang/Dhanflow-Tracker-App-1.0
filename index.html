import React, { useState, useEffect } from 'react';
import { Wallet, TrendingUp, TrendingDown, DollarSign, Trash2, Plus } from 'lucide-react';

export default function FinanceTracker() {
  const [salary, setSalary] = useState(0);
  const [expenses, setExpenses] = useState([]);
  const [expenseName, setExpenseName] = useState('');
  const [expenseAmount, setExpenseAmount] = useState('');
  const [showSalaryInput, setShowSalaryInput] = useState(true);

  const totalExpenses = expenses.reduce((sum, expense) => sum + expense.amount, 0);
  const remaining = salary - totalExpenses;
  const percentageUsed = salary > 0 ? (totalExpenses / salary * 100).toFixed(1) : 0;

  const addExpense = () => {
    if (expenseName && expenseAmount && parseFloat(expenseAmount) > 0) {
      setExpenses([...expenses, {
        id: Date.now(),
        name: expenseName,
        amount: parseFloat(expenseAmount)
      }]);
      setExpenseName('');
      setExpenseAmount('');
    }
  };

  const deleteExpense = (id) => {
    setExpenses(expenses.filter(expense => expense.id !== id));
  };

  const updateSalary = (value) => {
    setSalary(parseFloat(value) || 0);
    setShowSalaryInput(false);
  };

  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-50 to-indigo-100 p-4">
      <div className="max-w-4xl mx-auto">
        <div className="bg-white rounded-2xl shadow-xl p-6 mb-6">
          <div className="flex items-center gap-3 mb-6">
            <Wallet className="w-8 h-8 text-indigo-600" />
            <h1 className="text-3xl font-bold text-gray-800">Dhan Flow Tracker</h1>
          </div>

          {/* Salary Section */}
          <div className="bg-gradient-to-r from-indigo-500 to-purple-600 rounded-xl p-6 text-white mb-6">
            <div className="flex justify-between items-center">
              <div>
                <p className="text-indigo-100 text-sm mb-1">Monthly Salary</p>
                <p className="text-4xl font-bold">${salary.toFixed(2)}</p>
              </div>
              <button
                onClick={() => setShowSalaryInput(!showSalaryInput)}
                className="bg-white bg-opacity-20 hover:bg-opacity-30 px-4 py-2 rounded-lg transition"
              >
                Edit
              </button>
            </div>
            
            {showSalaryInput && (
              <div className="mt-4 flex gap-2">
                <input
                  type="number"
                  placeholder="Enter your salary"
                  className="flex-1 px-4 py-2 rounded-lg text-gray-800"
                  onKeyDown={(e) => {
                    if (e.key === 'Enter') updateSalary(e.target.value);
                  }}
                />
                <button
                  onClick={(e) => {
                    const input = e.target.previousSibling;
                    updateSalary(input.value);
                  }}
                  className="bg-white text-indigo-600 px-6 py-2 rounded-lg font-semibold hover:bg-indigo-50 transition"
                >
                  Set
                </button>
              </div>
            )}
          </div>

          {/* Summary Cards */}
          <div className="grid grid-cols-1 md:grid-cols-3 gap-4 mb-6">
            <div className="bg-red-50 rounded-xl p-4 border-2 border-red-100">
              <div className="flex items-center gap-2 mb-2">
                <TrendingDown className="w-5 h-5 text-red-600" />
                <p className="text-red-600 text-sm font-semibold">Total Expenses</p>
              </div>
              <p className="text-2xl font-bold text-red-700">${totalExpenses.toFixed(2)}</p>
            </div>

            <div className={`rounded-xl p-4 border-2 ${remaining >= 0 ? 'bg-green-50 border-green-100' : 'bg-red-50 border-red-100'}`}>
              <div className="flex items-center gap-2 mb-2">
                <DollarSign className={`w-5 h-5 ${remaining >= 0 ? 'text-green-600' : 'text-red-600'}`} />
                <p className={`text-sm font-semibold ${remaining >= 0 ? 'text-green-600' : 'text-red-600'}`}>Remaining</p>
              </div>
              <p className={`text-2xl font-bold ${remaining >= 0 ? 'text-green-700' : 'text-red-700'}`}>
                ${remaining.toFixed(2)}
              </p>
            </div>

            <div className="bg-blue-50 rounded-xl p-4 border-2 border-blue-100">
              <div className="flex items-center gap-2 mb-2">
                <TrendingUp className="w-5 h-5 text-blue-600" />
                <p className="text-blue-600 text-sm font-semibold">Budget Used</p>
              </div>
              <p className="text-2xl font-bold text-blue-700">{percentageUsed}%</p>
            </div>
          </div>

          {/* Add Expense Form */}
          <div className="bg-gray-50 rounded-xl p-4 mb-6">
            <h2 className="text-lg font-semibold text-gray-800 mb-3">Add Expense</h2>
            <div className="flex flex-col sm:flex-row gap-3">
              <input
                type="text"
                placeholder="Expense name"
                value={expenseName}
                onChange={(e) => setExpenseName(e.target.value)}
                className="flex-1 px-4 py-2 rounded-lg border-2 border-gray-200 focus:border-indigo-500 focus:outline-none"
              />
              <input
                type="number"
                placeholder="Amount"
                value={expenseAmount}
                onChange={(e) => setExpenseAmount(e.target.value)}
                onKeyDown={(e) => {
                  if (e.key === 'Enter') addExpense();
                }}
                className="w-full sm:w-32 px-4 py-2 rounded-lg border-2 border-gray-200 focus:border-indigo-500 focus:outline-none"
              />
              <button
                onClick={addExpense}
                className="bg-indigo-600 text-white px-6 py-2 rounded-lg font-semibold hover:bg-indigo-700 transition flex items-center justify-center gap-2"
              >
                <Plus className="w-5 h-5" />
                Add
              </button>
            </div>
          </div>

          {/* Expenses List */}
          <div>
            <h2 className="text-lg font-semibold text-gray-800 mb-3">Expenses</h2>
            {expenses.length === 0 ? (
              <p className="text-gray-500 text-center py-8">No expenses yet. Add your first expense above!</p>
            ) : (
              <div className="space-y-2">
                {expenses.map((expense) => (
                  <div
                    key={expense.id}
                    className="flex justify-between items-center bg-white border-2 border-gray-100 rounded-lg p-4 hover:border-gray-200 transition"
                  >
                    <div>
                      <p className="font-semibold text-gray-800">{expense.name}</p>
                      <p className="text-sm text-gray-500">${expense.amount.toFixed(2)}</p>
                    </div>
                    <button
                      onClick={() => deleteExpense(expense.id)}
                      className="text-red-600 hover:bg-red-50 p-2 rounded-lg transition"
                    >
                      <Trash2 className="w-5 h-5" />
                    </button>
                  </div>
                ))}
              </div>
            )}
          </div>
        </div>
      </div>
    </div>
  );
}
