Submit a single HTML file named enhanced-form.html. It should include:

Well-structured content using lists, tables, and media.

A complete HTML5 form including a variety of input fields.

Correct use of form attributes such as placeholder, required, autocomplete, and readonly.

HTML5 validation features implemented correctly across all relevant fields.

A clear, accessible layout using semantic tags.

answers.web
<!DOCKTYPE html>
    </style>
</head>
<body>

    <header>
        <h1>Website Showcase</h1>
    </header>

    <main>
        <section id="intro">
            <h2>About This Page</h2>
            <p>This document demonstrates a variety of HTML5 features as per the requirements. It includes:</p>
            <ul>
                <li>Semantic HTML for a clear and accessible layout.</li>
                <li>Embedded media (image) and tabular data.</li>
                <li>A comprehensive form with modern input types and validation.</li>
            </ul>
        </section>

        <section id="media-and-table">
            <h2>Event Information</h2>
            <article>
                <h3>Upcoming Workshop</h3>
                <img src="https://via.placeholder.com/760x200.png?text=HTML5+In+Action" alt="Banner for an HTML5 workshop">
                <p>Join our workshop to master modern web development techniques.</p>
            </article>
            <article>
                <h3>Workshop Schedule</h3>
                <table>
                    <caption>Daily Agenda</caption>
                    <thead>
                        <tr>
                            <th>Time</th>
                            <th>Topic</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>09:00 - 11:00</td>
                            <td>Semantic HTML & Accessibility</td>
                        </tr>
                        <tr>
                            <td>11:00 - 13:00</td>
                            <td>Advanced HTML5 Forms</td>
                        </tr>
                    </tbody>
                </table>
            </article>
        </section>

        <section id="registration-form">
            <h2>Registration Form</h2>
            <form action="#" method="post" autocomplete="on">
                <fieldset>
                    <legend>Personal Details</legend>

                    <label for="full-name">Full Name:</label>
                    <input type="text" id="full-name" name="full_name" placeholder="e.g., Jane Doe" required autocomplete="name">

                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" placeholder="you@example.com" required autocomplete="email">
                    
                    <label for="phone">Phone (optional):</label>
                    <input type="tel" id="phone" name="phone" placeholder="123-456-7890" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}" autocomplete="tel">
                </fieldset>

                <fieldset>
                    <legend>Account Information</legend>
                    
                    <label for="user-id">User ID (Assigned):</label>
                    <input type="text" id="user-id" name="user_id" value="REG-54321" readonly>

                    <label for="experience">Years of Web Dev Experience:</label>
                    <input type="number" id="experience" name="experience" min="0" max="50" required>

                    <label for="track">Desired Track:</label>
                    <select id="track" name="track" required>
                        <option value="">--Please choose an option--</option>
                        <option value="frontend">Front-End</option>
                        <option value="backend">Back-End</option>
                        <option value="fullstack">Full-Stack</option>
                    </select>
                </fieldset>

                <fieldset>
                    <legend>Preferences</legend>
                    <p>Notify me about:</p>
                    <label><input type="checkbox" name="interests" value="html_css"> HTML/CSS News</label>
                    <label><input type="checkbox" name="interests" value="javascript"> JavaScript Updates</label>
                    <label><input type="checkbox" name="interests" value="backend"> Back-End Technologies</label>
                </fieldset>

                <button type="submit">Submit Registration</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Enhanced Forms Inc.</p>
    </footer>

</body>
</html>
