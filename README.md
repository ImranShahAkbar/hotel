Its Project Where i HAVE used 
1. Guest Table
export class Guest {
  guest_guestID: number | undefined;
  guest_name: string | undefined;
  guest_address: string | undefined;
  guest_phone: string | undefined;
  guest_nid: string | undefined;
}
2. Room_Type Table
export class RoomType {
  roomtype_typeID: number | undefined;
  roomtype_name: string | undefined;
  roomtype_description: string | undefined;
  roomtype_rentPerNight: number | undefined;
}
3. Room Table
export class Room {
  room_roomID: number | undefined;
  room_roomNo: string | undefined;
  room_roomTypeID: number | undefined;
  room_status: string | undefined;
}
4. Booking Table
export class Booking {
  booking_bookingID: number | undefined;
  booking_guestID: number | undefined;
  booking_roomID: number | undefined;
  booking_checkInDate: string | undefined;
  booking_checkOutDate: string | undefined;
  booking_nights: number | undefined;
}
5. Invoice Table
export class Invoice {
  invoice_invoiceID: number | undefined;
  invoice_bookingID: number | undefined;
  invoice_invoiceDate: string | undefined;
  invoice_serviceCharge: number | undefined;
  invoice_vat: number | undefined;
  invoice_totalAmount: number | undefined;
}
6. Payment Table
export class Payment {
  payment_paymentID: number | undefined;
  payment_invoiceID: number | undefined;
  payment_paymentDate: string | undefined;
  payment_amount: number | undefined;
  payment_paymentMethod: string | undefined;
  payment_transactionID: string | undefined;
}
7. Expense_Category Table
export class ExpenseCategory {
  expensecategory_categoryID: number | undefined;
  expensecategory_name: string | undefined;
}
8. Staff Table
export class Staff {
  staff_staffID: number | undefined;
  staff_name: string | undefined;
  staff_designation: string | undefined;
}
9. Expense Table
export class Expense {
  expense_expenseID: number | undefined;
  expense_staffID: number | undefined;
  expense_categoryID: number | undefined;
  expense_expenseDate: string | undefined;
  expense_amount: number | undefined;
  expense_description: string | undefined;
}
10. Daily_Transaction Table
export class DailyTransaction {
  dailytransaction_transactionID: number | undefined;
  dailytransaction_transactionDate: string | undefined;
  dailytransaction_type: string | undefined;
  dailytransaction_amount: number | undefined;
  dailytransaction_vat: number | undefined;
}
11. Profit_Loss_Summary Table
export class ProfitLossSummary {
  profitloss_recID: number | undefined;
  profitloss_date: string | undefined;
  profitloss_totalIncome: number | undefined;
  profitloss_totalExpense: number | undefined;
  profitloss_profitOrLoss: number | undefined;
}
12. Tour_Package Table
export class TourPackage {
  tourpackage_packageID: number | undefined;
  tourpackage_name: string | undefined;
  tourpackage_description: string | undefined;
  tourpackage_basePrice: number | undefined;
  tourpackage_location: string | undefined;
}
13. Tour_Booking Table
export class TourBooking {
  tourbooking_tourBookingID: number | undefined;
  tourbooking_guestID: number | undefined;
  tourbooking_packageID: number | undefined;
  tourbooking_tourDate: string | undefined;
  tourbooking_noOfPeople: number | undefined;
}
14. Tour_Invoice Table
export class TourInvoice {
  tourinvoice_tourInvoiceID: number | undefined;
  tourinvoice_bookingID: number | undefined;
  tourinvoice_invoiceDate: string | undefined;
  tourinvoice_vat: number | undefined;
  tourinvoice_totalAmount: number | undefined;
}
