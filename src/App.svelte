<script>
    import { Col, Row, Media } from "sveltestrap";
    import Card from "./Card/Card.svelte";
    import Carousel from "./Carousel/Carousel.svelte";
    import Footer from "./Footer/Footer.svelte";
    import NavigatorBar from "./Navbar/NavigatorBar.svelte";
</script>

<main>
    <NavigatorBar />
    <Carousel />
    <h1 class="text-center">What we offer</h1>
    <div class="container mt-5">
        <Row>
            <Col xs="6"><img src="../img/woman.png" alt="Woman" style="height: 540px; width: 550px;" /></Col>
            <Col xs="6">
                <div class="aStyle">
                    <h5 class="tittleStyle">
                        <strong class="firstStyle"> Online Courses</strong>
                        <span> <br>Our Course are the best among others</span> ?
                    </h5>
                    <p>
                        Lorem ipsum dolor sit at, consectetur adipielit. Facilisi fermentum, 
                        dignissim pharetra. Aliquam Lorem ipsum dolor sit at, consectetur adipielit. Facilisi fermentum, dignissim pharetra. Aliquam 
                    </p>
                    <a href="#!" class="text-danger">Explore our courses</a>
                </div>
            </Col>
        </Row>
    </div>

    <div class="container mt-5 mb-5">
        <Row>
            <Col xs="6">
                <div class="bStyle">
                    <p>
                        Lorem, ipsum dolor sit amet consectetur adipisicing
                        elit. Rem expedita, neque nihil eius et assumenda!
                        Libero vero magnam cumque voluptatum aut, commodi
                        tenetur maxime incidunt fuga ea asperiores ab autem!
                    </p>
                </div>
            </Col>
            <Col xs="6"
                ><img
                    class="humansOne"
                    src="../img/humans1.png"
                    alt="Gambar 1"
                /></Col
            >
        </Row>
    </div>

    <Footer />
</main>

<style>
     h1 {
        text-align: center;
        margin-top: 20px;
    }
    .aStyle {
        margin-top: 45px;
    }
    .bStyle {
        margin-top: 90px;
    }
    .tittleStyle {
        font-size: 45px;
    }
    .firstStyle {
        color: darkcyan;
        font-size: 50px;
    }
    .humansOne {
        margin-left: 90px;
        width: 450px;
        height: 350px;
    }
</style>
