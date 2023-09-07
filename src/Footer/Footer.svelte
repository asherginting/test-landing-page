<script>
    import { Col, Row } from "sveltestrap";

    let _tahun = new Date().getFullYear();
</script>

<footer class="bg-primary text-white text-lg-start">
    <!-- Grid container -->
    <div class="container-fluid py-5">
        <!--Grid row-->
        <Row>
            <!--Grid column-->
            <Col xl="6" xs="12">
                <img src="../img/logo-white.png" alt="Logo" style="height: 20px; width: 100px; margin-left: 70px" />

                <p style="margin-left: 70px; margin-top: 10px">
                    We are not here to sell you products, we sell value through our expertise.
                </p>
            </Col>
            <!--Grid column-->

            <!--Grid column-->
            <Col xl="3" xs="6">
                <h6>Address</h6>

                <ul class="list-unstyled">
                    <li>
                        <a href="#!" class="text-white">38 opebi Road, Ikeja, Lagos State, Nigeia.</a>
                    </li>
                </ul>
            </Col>
            <!--Grid column-->

            <!--Grid column-->
            <Col xl="3" xs="6">
                <h6>Company</h6>

                <ul class="list-unstyled  mb-0">
                    <li>
                        <a href="#!" class="text-white">About Us</a>
                    </li>
                    <li>
                        <a href="#!" class="text-white">Features</a>
                    </li>
                    <li>
                        <a href="#!" class="text-white">Pricing</a>
                    </li>
                </ul>
            </Col>
            <!--Grid column-->
        </Row>
        <!--Grid row-->
    </div>
    <!-- Grid container -->

    <!-- Copyright -->
    <div class="text-center p-3 footerStyle">
        © {_tahun} By Asher Azriel Ginting
    </div>
    <!-- Copyright -->
</footer>

<style>
    .bg-primary {
        background-color: #1B353D !important;
    }
    .footerStyle {
        background-color: rgba(0, 0, 0, 0.2);
    }
</style>
