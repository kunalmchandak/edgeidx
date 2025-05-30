#   edgeIDX

##   Overview

    edgeIDX is a Python package for extracting Aadhaar card details (Name, DOB, Gender, and Aadhaar Number) from images using Tesseract OCR. Unlike traditional setups, this package embeds a trained Tesseract model within itself, eliminating the need for a separate `tesseract.exe` installation.

    This project aims to address the limitations of existing OCR systems by focusing on accuracy, speed, and lightweight deployment. It is specifically designed for extracting information from government-issued identity documents such as Aadhaar and PAN cards.

##   Features

* Extracts Aadhaar card details (Name, DOB, Gender, and Aadhaar Number) from images using OCR.
* Uses an embedded Tesseract model, requiring no external dependencies.
* Supports image preprocessing to improve OCR accuracy.
* Works across different platforms without requiring external Tesseract installation.
* Can be integrated with Android applications for automated Aadhaar data extraction.


* **High Accuracy OCR:** Achieves over 95% accuracy in extracting key details such as names, dates of birth, and ID numbers.
* **Real-Time Processing:** Processes each document within 1-2 seconds to facilitate high-throughput applications.
* **Edge Device Compatibility:** Designed for low-resource environments like mobile phones.
* **Open-Source and Developer-Friendly:** Provides a modular, open-source library with clear documentation.
* **JSON Output Format:** Extracted details are formatted in JSON for seamless integration into different applications.
* **Compliance with Data Privacy Regulations:** Ensures that the extracted information is handled securely and adheres to laws such as Aadhaar Act, 2016, Personal Data Protection Bill, 2021, and General Data Protection Regulation (GDPR).
* **Future-Proof Design:** The modular architecture allows easy integration of additional document types in future releases.

##   System Requirements

* Python 3.7+
* OpenCV for image processing
* NumPy for handling image arrays
* Pytesseract for OCR
* Supported Operating Systems: Windows and Linux.
* Supported Edge Devices: Mobile phones, Raspberry Pi, and other low-power devices.
* Development Frameworks: OpenCV, and Tesseract-OCR.

##   Installation

###   1\. Install via pip 

    ```sh
    pip install edgeidx
    ```

##   Usage



    ```python
    #   Example Usage (Adapt this to your library's API)
    from edgeidx.ocr import extract_aadhaar_details

    image_path = "sample_13.jpg"
    print(extract_aadhaar_details(image_path))
    ```

##   Output Format

The extracted data is returned in JSON format:

    ```json
    {
        "name": "John Doe",
        "date_of_birth": "01/01/1990",
        "gender": "Male",
        "aadhaar_number": "XXXX-XXXX-XXXX"
    }
    ```


##   Constraints

* **Compliance with Data Protection Laws:** The system must follow Aadhaar Act, GDPR, and data privacy regulations.
* **Lightweight Execution:** The model must be optimized for low-power devices through pruning, quantization, and efficient memory usage.

##   Non-Functional Requirements

* **Performance:**
    * Ensure OCR accuracy > 95%.
    * Processing time per document: 1-2 seconds.

* **Usability:**
    * Provides clear API documentation and sample integration examples.

* **Software Quality Attributes:**
    * Efficiency: Optimized for low-latency execution.
    * Scalability: Supports additional document types with minimal modifications.

##   Use Cases

* **Developers:** Integrate edgeIDX into their applications using provided APIs and libraries.
* **Businesses:** Automate document verification processes to improve efficiency in sectors like banking, healthcare, and telecom.
* **Prototype Developers:** Using Python Library for research


##   Team

* Kunal Chandak [kunalmchandak](https://github.com/kunalmchandak)
* Mayuresh Muluk [Mayuresh28](https://github.com/Mayuresh28)

##   References

* Aadhaar Act, 2016: Legal guidelines for handling Aadhaar data in India.
* Personal Data Protection Bill, 2021: Regulations related to sensitive personal data processing.
* General Data Protection Regulation (GDPR): European data privacy and protection regulations.

##   Conclusion

    edgeIDX is an open-source, high-accuracy OCR system optimized for government-issued documents. It offers fast processing, modular design, and edge-device compatibility, making it a valuable contribution to the open-source community.
    
