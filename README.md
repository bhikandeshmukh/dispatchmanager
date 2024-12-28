# Dispatch Manager

## Overview
The **Dispatch Manager** is a web-based application designed to streamline the process of managing dispatches, returns, and cancellations for various e-commerce portals and courier services. It includes features such as barcode scanning, data entry, bulk deletion, and data export to Excel. The application is built using HTML, CSS, and JavaScript, with additional libraries for barcode scanning (Quagga), Excel export (XLSX), and toast notifications (Toastify).

## Features
1. **Portal and Courier Selection**:  
   - Choose from popular e-commerce portals like Flipkart, Myntra, Meesho, Amazon, Amazon Flex, and Snapdeal.  
   - Select courier services such as Ekart, Shadowfax, Delhivery, Xpressbees, Ecom Express, ATS, and BlueDart.  

2. **Scan Type**:  
   - Supports three scan types: Dispatch, Return, and Cancel.  

3. **Barcode Scanning**:  
   - Scan barcodes using the device's camera (preferably the rear camera).  
   - Supports Code 128 and Code 39 barcodes.  
   - Automatically saves scanned data to the table.  

4. **Manual Data Entry**:  
   - Enter tracking IDs manually if barcode scanning is not available.  

5. **Live Scanned Data Table**:  
   - Displays scanned data in a table with columns for Date, Portal, Dispatch Type, Tracking ID, and Courier.  
   - Allows bulk deletion of selected entries.  

6. **Data Export**:  
   - Export the scanned data to an Excel file (XLSX format).  

7. **Dark Mode**:  
   - Toggle between light and dark themes for better visibility in low-light environments.  

8. **Clear All Data**:  
   - Clear all entries from the table with a single click.  

9. **Error Handling**:  
   - Displays error messages for invalid or duplicate barcodes.  

10. **Responsive Design**:  
    - Optimized for both desktop and mobile devices.  

## How to Use
1. **Select Portal, Courier, and Scan Type**:  
   - Use the dropdown menus to select the appropriate portal, courier, and scan type.  

2. **Scan Barcode or Enter Tracking ID**:  
   - Click on the camera feed to start scanning barcodes.  
   - Alternatively, manually enter the tracking ID in the input field and click "Save."  

3. **View and Manage Data**:  
   - Scanned data will appear in the table below.  
   - Use the checkboxes to select entries for bulk deletion.  

4. **Export Data**:  
   - Click the "Download as XLSX" button to export the table data to an Excel file.  

5. **Toggle Dark Mode**:  
   - Click the "Toggle Dark Mode" button to switch between light and dark themes.  

6. **Clear All Data**:  
   - Use the "Clear All Data" button to remove all entries from the table.  

## Libraries Used
- **Quagga**: For barcode scanning.  
- **XLSX**: For exporting data to Excel.  
- **Toastify**: For displaying toast notifications.  
- **Font Awesome**: For icons.    

## Notes
- The application uses the device's rear camera for barcode scanning. If the rear camera is not available, it will default to the front camera.  
- For optimal performance, use a device with a high-resolution camera and good lighting conditions.  
- The beep sound is played on successful barcode scanning. Ensure the `beep.wav` file is in the same directory as the HTML file.  

## Author
**Bhikan Deshmukh**  

## License
This project is open-source and available under the MIT License.  

---

Feel free to contribute or report issues!
