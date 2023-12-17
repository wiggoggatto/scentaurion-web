<script>
    // Define the content for each column
    let column1Content = "About Us";
    let column2Content = "Contact Us";
    let column3Content = "Social Media";

</script>

<style>
    .footer {
        display: flex;
        justify-content: space-between;
        background-color: #8A2BE2;
        color: white;
        padding: 20px;
    }

    .column {
        flex: 1;
        margin-right: 20px;
    }
</style>

<div>
    <div class="footer">
        <div class="column">
            <h3>${column1Content}</h3>
            <ul>
                <li>About</li>
                <li>Our Story</li>
                <li>Team</li>
            </ul>
        </div>
        <div class="column">
            <h3>${column2Content}</h3>
            <ul>
                <li>Contact Info</li>
                <li>Email</li>
                <li>Phone</li>
            </ul>
        </div>
        <div class="column">
            <h3>${column3Content}</h3>
            <ul>
                <li>Facebook</li>
                <li>Instagram</li>
                <li>Twitter</li>
            </ul>
        </div>
    </div>
    <footer class="footer">
        <p>&copy; 2022 Perfume World. All rights reserved.</p>
    </footer>
</div>
