## description ##
The frontend is designed to run locally, interacting with an API to provide dynamic functionality such as getting and displaying locations, location-specific details, and loading common elements such as headers and footers.

---

## **Prerequisites**

1. **Python 3**: Make sure you have Python 3 installed on your system.
2. **Development Environment**: A text editor such as **Visual Studio Code** (optional).
3. **Web Browser**: Any modern browser.

---

## **How ​​to run the project locally**

1. **Clone the repository**
Open a terminal and clone this repository to your local machine:

git clone git@github.com:smorkl/newhbnb.git

2. **Navigate to the project directory**

cd /path/to/your/project

3. **Start a local server**
Use the following command to start the HTTP server:

python3 -m http.server 5500

4. **Access the project from your browser**
Open your web browser and visit the following address:

http://localhost:5500

Note: Make sure that port 5500 is not in use for another process before starting the server.

----

## **The frontend allows the user to:**

1. **Get and view places**

View a list of available places.
Filter places by price.
View images associated with each place to make the browsing experience easier.

2. **Place details**
When you select a place, a specific page is displayed that includes:

owner name
Detailed description of the place.
Price per night.
List of services and amenities.
Representative image of the place.

3. **Dynamic loading of header and footer**
To facilitate consistency across project pages:

The header and footer are dynamically loaded from external files using JavaScript.
This improves modularity and makes code maintenance easier.

*IMPORTAN*
**You have to keep in mind that these depend on a backend which is located in this same repository. You can use these commands to get to it**

cd ..
cd ..
cd part 2 and 3
back of cd