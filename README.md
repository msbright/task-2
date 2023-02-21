# task-2
Xxxxx
import java.text.DecimalFormat;
import java.util.Scanner;

public class Account {
	Scanner input = new Scanner(System.in);
	DecimalFormat moneyFormat = new DecimalFormat("'$'###,##0.00");

	/* Set the customer number */

	public int setCustomerNumber(int customerNumber) {
		this.customerNumber = customerNumber;
		return customerNumber;
	}

	/* Get the customer number */

	public int getCustomerNumber() {
		return customerNumber;
	}

	/* Set the pin number */

	public int setPinNumber(int pinNumber) {
		this.pinNumber = pinNumber;
		return pinNumber;
	}

	/* Get the pin number */

	public int getPinNumber() {
		return pinNumber;
	}

	/* Get Current Account Balance */

	public double getCurrentBalance() {
		return currentBalance;
	}

	/* Get Saving Account Balance */

	public double getSavingBalance() {
		return savingBalance;
	}

	/* Calculate Current Account withdrawal */

	public double calCurrentWithdraw(double amount) {
		currentBalance = (currentBalance - amount);
		return currentBalance;
	}

	/* Calculate Saving Account withdrawal */

	public double calSavingWithdraw(double amount) {
		savingBalance = (savingBalance - amount);
		return savingBalance;
	}

	/* Calculate Current Account deposit */

	public double calCurrentDeposit(double amount) {
		currentBalance = (currentBalance + amount);
		return currentBalance;
	}

	/* Calculate Saving Account deposit */

	public double calSavingDeposit(double amount) {
		savingBalance = (savingBalance + amount);
		return savingBalance;
	}
	
	/* Customer Transfer Amount from Saving Account */

	public double calSavingTransfer(double amount) {
		savingBalance = (savingBalance - amount);
		return savingBalance;
	}

	/* Customer Deposit Transfer Amount from Saving to Current Account */

	public double calCurrentTransfer(double amount) {
		currentBalance = (currentBalance + amount);
		return currentBalance;
	}


	/* Customer Current Account Withdraw input */
