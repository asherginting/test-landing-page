<script>
    import {
        Collapse,
        Navbar,
        NavbarToggler,
        NavbarBrand,
        Nav,
        NavItem,
        NavLink,
        UncontrolledDropdown,
        DropdownToggle,
        DropdownMenu,
        DropdownItem,
        Button,
    } from "sveltestrap";

    let isOpen = false;

    function handleUpdate(event) {
        isOpen = event.detail.isOpen;
    }
</script>

<Navbar color="white" dark expand="md" class="fixed-top">
    <NavbarBrand href="/">
        <img src="../img/logo.png" alt="Logo" style="height: 20px; width: 100px; margin-left: 70px" />
    </NavbarBrand>    
    <NavbarToggler on:click={() => (isOpen = !isOpen)} />
    <Collapse {isOpen} navbar expand="md" on:update={handleUpdate}>
        <Nav class="ml-auto mr-5 py-2" navbar>
            <NavItem class="ml-4">
                <NavLink href="#!" style="color: gray;">Home</NavLink>
            </NavItem>
            <NavItem class="ml-4">
                <NavLink href="#!" style="color: gray;">Courses</NavLink>
            </NavItem>
            <NavItem class="ml-4">
                <NavLink href="#!" style="color: gray;">Instructor</NavLink>
            </NavItem>
            <NavItem class="ml-4">
                <NavLink href="#!" style="color: gray;">Schedules</NavLink>
            </NavItem>
            <NavItem class="ml-4">
                <NavLink href="#!" style="color: gray;">Contact Us</NavLink>
            </NavItem>

            <NavItem class="ml-4">
                <form class="form-inline">
                    <div class="input-group">
                        <input type="text" class="form-control" placeholder="Search" />
                        <div class="input-group-append">
                            <button class="btn btn-outline-secondary" type="button">
                                <img src="../icon/search.png" alt="Logo" style="height: 20px; width: 20px;" />
                            </button>
                        </div>
                    </div>
                </form>
            </NavItem>

            <a href="#!" class="btn ml-4" style="color: gray;"
                >
                <img src="../icon/profile.png" alt="Logo" style="height: 30px; width: 30px;" />
                </a
            >
        </Nav>
    </Collapse>
</Navbar>

<style>
    .buttonStyle {
        border-radius: 20px;
        background-color: orange;
        color: white;
    }
    .buttonStyle:hover {
        border-radius: 20px;
        background-color: orange;
        color: white;
    }
</style>
