# SAP UI5 Invoice Browser

This project is a demo **SAPUI5 web application** for browsing and inspecting invoice data using the public Northwind OData service. It demonstrates a typical MVC architecture, routing, internationalization, data binding, and integration with mock and remote data services.

---

## Prerequisites

To run this project, you need the following tools installed on your machine:

- [Node.js](https://nodejs.org/) (for UI5 Tooling)
- [UI5 CLI](https://sap.github.io/ui5-tooling/) (`npm install --global @ui5/cli`)

---

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/pohbl4/Sapui5-invoice-demo.git
   cd Sapui5-invoice-demo
   ```

2. Install dependencies (if any):
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   ui5 serve -o
   ```

   This will open the application in your default browser.

---

## How It Works

### Application Features

- **Invoice List View:** Displays a searchable list of invoices retrieved from the Northwind OData service.
- **Invoice Detail View:** Navigates to a detail view of the selected invoice.
- **Hello Panel:** A basic interactive example with i18n support and a dialog popup.
- **Routing:** Configured to navigate between views using URL hashes.
- **Mock Server:** Available for development without relying on live OData.
- **i18n:** Built-in internationalization for UI text.

### Folder Structure

- `webapp/controller/` — Controllers for each view (App, Detail, InvoiceList, HelloPanel)
- `webapp/view/` — XML views corresponding to each controller
- `webapp/model/formatter.js` — Helper for formatting invoice status
- `webapp/localService/` — Mock server and metadata for development
- `webapp/test/` — Integration and unit tests using QUnit and OPA

---

## Example Use Case

1. The app launches with a list of invoices.
2. You can filter the invoices by product name.
3. Click on an invoice to view its details.
4. Optionally, open the "Hello" dialog as a UI demonstration.

