# BIZCARDX
Project Overview:

                The "BizCard" project aims to simplify the process of extracting and managing information from business cards. With this application, users can upload an image of a business card, extract relevant details using Optical Character Recognition (OCR), and display the extracted data. Additionally, users have the option to store the extracted information in a MySQL database for easy access and management. The project utilizes various libraries such as pandas, numpy, streamlit, easyocr, PIL, cv2, and re to achieve its functionalities.

Workflow:

1. Imported the necessary libraries for the project, including pandas, streamlit, easyocr, PIL, base64,  cv2, and re.

2. Set up the required configurations and established  a connection with the MySQL database.

3. Created a dictionary to store the extracted data, including fields such as name, designation, mobile number, company name, email ID, website, area, city, state, Pincode, and image.

4. Developed  the user interface using Streamlit. Created different pages for the application: "HOME," "DISPLAY," and "MODIFY."

5. In the "HOME" page, displays  a welcome message and provides instructions for the user to upload an image of a business card using the sidebar.

6. In the "DISPLAY" page, check if an image has been uploaded. The image is  preprocessed  using OpenCV and used OCR to extract the text. Extracted specific information from the OCR results, such as name, designation, mobile number, email ID, website, area, city, state, and pincode.

7.  Extracted information was stored  in the dictionary created earlier.

8. Created a DataFrame using pandas to organize the extracted data.

9. Displays the extracted data in an interactive table using the AgGrid library, which allows the  users to view and modify the information if needed.

10. Provided a button labeled "UPLOAD TO DB" to allow users to upload the extracted data to the MySQL database. 

11. In the "MODIFY" page,  users were given  the option to update or delete information from the database by providing  a select box to choose between "UPDATE" and "DELETE."

12. If "UPDATE" is selected,  the existing information for a specific person from the database is retrieved. The retrieved information is displayed and  users  were allowed to update the desired fields. On submission,  the corresponding records were updated  in the "businesscard" table.

13. If "DELETE" is selected,  the existing information for a specific person from the database were retrieved.  The retrieved information was displayed and provided a button labeled "DELETE" to remove the record from the database.


With this project workflow, users can effortlessly extract information from business cards, view and modify the extracted data, and store it in a MySQL database for efficient management and future reference.

 

