<template>
    <div class="contact">
        <div class="background"></div>
        <div class="container my-5">
            <div class="row">
                <div class="col-md-6 text-light my-auto">
                    <h2>Want to give us feedback? Want to learn more?</h2>
                    <p>We'd love to hear from you!</p>
                </div>
                <div class="col-md-6">
                    <div class="row" style="background-color: white; border-radius: 20px;">
                        <div class="col-2" style="background-color: #F48E72; border-bottom-left-radius: 20px; border-top-left-radius: 20px;"></div>
                        <div class="col-10">
                            <form action="https://formspree.io/contact@funnelfoods.com" method="POST" class="my-5 text-left">
                                <h1>Send us a message</h1>
                                <div class="form-row">
                                    <div class="col-md-6 mb-3">
                                        <label for="first-name">First name</label>
                                        <input name="first-name" class="form-control" id="first-name" placeholder="First name" value="Mark" required>
                                        <div class="valid-feedback">
                                            Looks good!
                                        </div>
                                    </div>
                                    <div class="col-md-6 mb-3">
                                        <label for="last-name">Last name</label>
                                        <input name="last-name" class="form-control" id="last-name" placeholder="Last name" value="Otto" required>
                                        <div class="valid-feedback">
                                            Looks good!
                                        </div>
                                    </div>
                                </div>
                                <div class="form-row">
                                    <div class="col-md-12 mb-3">
                                        <label for="email">Email</label>
                                        <input name="_replyto" type="text" class="form-control" id="email" placeholder="Email" required>
                                        <div class="invalid-feedback">
                                            Please provide a valid email.
                                        </div>
                                    </div>
                                </div>
                                <div class="form-row">
                                    <div class="col-md-12 mb-3">
                                        <label for="title">Title</label>
                                        <input name="title" class="form-control" id="title" placeholder="Title" required>
                                        <div class="invalid-feedback">
                                            Please provide a valid title.
                                        </div>
                                    </div>
                                </div>
                                <div class="form-row">
                                    <div class="col-md-12 mb-3">
                                        <label for="message">Message</label>
                                        <textarea name="message" rows="6" class="form-control" id="message" placeholder="Message" style="resize: none;" required>

                                        </textarea>
                                        <div class="invalid-feedback">
                                            Please provide a valid message.
                                        </div>
                                    </div>
                                </div>
                                <div class="form-row">
                                    <input type="submit" value="Submit" class="btn btn-outline-info"/>
                                </div>
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Contact",
        metaInfo: {
            title: 'FunnelFoods | Contact',
            // Define meta tags here.
        }
    }
</script>

<style >
    .background {
        position: absolute;
        top: 0;
        left: 0;
        background-image: linear-gradient(#1d3e62, #aad3cc);
        z-index: -1;
        width: 100%;
        height: 100%;
    }
    .nav-link {
        color: white;
    }
</style>
