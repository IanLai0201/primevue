<template>
    <div>
        <Head>
            <Title>Bootstrap - PrimeVue</Title>
            <Meta name="description" content="Styling PrimeVue with Boostrap." />
        </Head>

        <div class="doc">
            <div class="doc-main">
                <div class="doc-intro">
                    <h1>Bootstrap</h1>
                    <p>Boostrap is a well-known CSS library to build responsive and mobile first web projects.</p>
                </div>
                <DocSections :docs="docs" />
            </div>
            <DocSectionNav :docs="docs" />
        </div>
    </div>
</template>

<script>
import ExampleDoc from '@/doc/bootstrap/ExampleDoc';
import SetupDoc from '@/doc/bootstrap/SetupDoc';

export default {
    data() {
        return {
            docs: [
                {
                    id: 'setup',
                    label: 'Setup',
                    component: SetupDoc
                },
                {
                    id: 'example',
                    label: 'Example',
                    component: ExampleDoc
                }
            ]
        };
    }
};
</script>
