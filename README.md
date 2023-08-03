# UpSchool-CapstoneProject
 
https://github.com/aycakbas/UpSchool-CapstoneProject/assets/121265757/b3d218f8-23ad-48c2-ad2e-0e8e4c5df7cf

<h2>Description</h2>
<p>Crawler Bot is a C# .NET project designed to scrape product information from an e-commerce website and store it in a MySQL database. It utilizes a C# background worker to navigate the target website and extract details such as product names, prices, discount availability, and image URLs. The project follows the Clean Architecture and CQRS design patterns, ensuring a well-structured and maintainable codebase.</p>
<h2>Features</h2>
<p><b>Web scraping of product details:</b> The Crawler Bot navigates to the e-commerce website and gathers product information, including regular and discounted prices, image URLs, and product names.</p>
<p><b>Clean Architecture and CQRS:</b> The project is structured according to the Clean Architecture principles, ensuring separation of concerns and maintainability. The CQRS pattern is implemented to segregate read and write operations effectively.</p>
<p><b>User Management:</b> Microsoft Identity is employed for user authentication, allowing users to register and log in through traditional methods or using Google login. JWT tokens are used for secure login/logout procedures.</p>
<p><b>Email Notifications:</b> The application sends email notifications to users upon registration and when specific product details are scraped.</p>
<p><b>Global Exception Handling:</b> A GlobalException filter is implemented to handle and manage exceptions gracefully throughout the application.</p>
<p><b>Front-end with React and TypeScript:</b> The front-end of the application is built using React with TypeScript, providing a responsive and user-friendly interface.</p>
<p><b>Tailwind CSS for Styling:</b> Tailwind CSS is used for designing the UI, ensuring a clean and modern appearance.</p>
<h2>Back-end Technologies</h2>
<p>C# .NET</p>
<p>Clean Architecture</p>
<p>CQRS (Command Query Responsibility Segregation)</p>
<p>Microsoft Identity for User Management</p>
<p>JWT (JSON Web Tokens) for Authentication</p>
<p>MySQL for Database Management</p>
<p>Background Worker for Web Scraping</p>
<p>SignalR for Real-Time Communication</p>
<p>Selenium Framework for bots</p>
<h2>Front-end Technologies</h2>
<p>React with TypeScript</p>
<p>Tailwind CSS for Styling</p>
<h2>How the Crawler Bot Works</h2>
<p><b>User Authentication:</b> Users can register and log in using traditional methods or through Google login. JWT tokens are issued for secure authentication.</p>
<p><b>Homepage:</b> Upon successful login, users are directed to the home page, where they can directly navigate to give an order.</p>
<p><b>Creating Orders:</b> Users can create new orders, specifying details such as the number of products to scrape and the type of products (all, discounted, non-discounted).</p>
<p><b>SignalR Communication:</b> When an order is created, the details are sent to the back-end worker using SignalR hub for web scraping.</p>
<p><b>Web Scraping:</b> The background worker, with the help of a web driver, navigates to the e-commerce website and performs web scraping based on the user's order details.</p>
<p><b>Data Storage:</b> The scraped product information is stored in the "Product" table, and order-related information is stored in the "Order" table. Bot status and order completion details are saved in the "Order Event" table.</p>
<p><b>Live Tracking:</b> Users can track the bot's progress and the scraped products in real-time using the "Live Track" page. SignalR facilitates the transfer of logs from the back-end to the front-end for live updates.</p>
<p><b>Protected Routes:</b> The application uses protected routes to ensure user session security. If a token expires, the user is automatically logged out for enhanced security.</p>
<h2>Email Notification and Export to Excel</h2>
<p>Users have the option to export their order details to an Excel table directly from the product page and send these crawled products via email. This feature enables users to conveniently analyze, store, and share their scraped data with ease.</p>
<h2>Installation and Setup</h2>
<p>Clone the repository from GitHub.</p>
<p>Set up the necessary environment for C# .NET and React with TypeScript.</p>
<p>Install the required C# and JavaScript dependencies.</p>
<p>Configure the MySQL database connection settings.</p>
<p>Build and run the C# .NET back-end.</p>
<p>Start the React front-end to access the Crawler Bot application.</p>
