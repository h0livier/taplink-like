<script setup lang="ts">
import { LinkBasic, LinkBrand } from '#components';
import Title from '~/components/title.vue';
</script>
<template>
    <main class="flex justify-center py-10 bg-[#1F1D21] md:bg-[#2C2A30] min-h-screen">
        <div class="md:bg-[#1F1D21] md:shadow-md md:rounded-lg pt-10 px-5 w-[95vw] md:w-[50vw] lg:w-[40vw] xl:w-[30vw]">
            <div>
                <div class="avatar">
                    <div class="w-32 rounded-full">
                        <img src="../assets/picture_squared.jpg" class="" alt="Olivier Hayot" />
                    </div>
                </div>
                <h1 class="text-3xl font-bold mt-4">Olivier Hayot</h1>
                <p class="text-xl text-gray-300">Analyste Développeur</p>
            </div>
            <div>
                <Section>
                    <Title text="Portfolio" />
                    <LinkBrand image="linkedin" text="Mon Linkedin"link="https://www.linkedin.com/in/olivier-hayot/" />
                    <LinkBrand image="github" text="Mon Github" link="https://github.com/h0livier" />
                </Section>
                <Section>
                    <Title text="Informations de contact" />
                    <LinkBasic title="Email" text="olivier.hayot.dev@gmail.com" link="mailto:olivier.hayot.dev@gmail.com" />
                    <LinkBasic title="Site Web" link="https://www.olivierhayot.be" />
                    <LinkBasic title="Mon CV" badge-text="Nouveau" link="https://cv.olivierhayot.be/" />
                </Section>
            </div>
        </div>
    </main>
</template>