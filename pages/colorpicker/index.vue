<template>
    <DocComponent title="Vue ColorPicker Component" header="ColorPicker" description="ColorPicker is an input component to select a color." :componentDocs="docs" :apiDocs="['ColorPicker']" :ptTabComponent="ptComponent" />
</template>

<script>
import AccessibilityDoc from '@/doc/colorpicker/AccessibilityDoc';
import BasicDoc from '@/doc/colorpicker/BasicDoc';
import DisabledDoc from '@/doc/colorpicker/DisabledDoc';
import FormatDoc from '@/doc/colorpicker/FormatDoc';
import ImportDoc from '@/doc/colorpicker/ImportDoc';
import InlineDoc from '@/doc/colorpicker/InlineDoc';
import StyleDoc from '@/doc/colorpicker/StyleDoc';
import VeeValidateDoc from '@/doc/colorpicker/form/VeeValidateDoc';
import PTComponent from '@/doc/colorpicker/pt/index.vue';

export default {
    data() {
        return {
            docs: [
                {
                    id: 'import',
                    label: 'Import',
                    component: ImportDoc
                },
                {
                    id: 'basic',
                    label: 'Basic',
                    component: BasicDoc
                },
                {
                    id: 'inline',
                    label: 'Inline',
                    component: InlineDoc
                },
                {
                    id: 'format',
                    label: 'Format',
                    component: FormatDoc
                },
                {
                    id: 'disabled',
                    label: 'Disabled',
                    component: DisabledDoc
                },
                {
                    id: 'form',
                    label: 'Form',
                    description: 'Compatibility with popular Vue form libraries.',
                    children: [
                        {
                            id: 'veevalidate',
                            label: 'VeeValidate',
                            component: VeeValidateDoc
                        }
                    ]
                },
                {
                    id: 'style',
                    label: 'Style',
                    component: StyleDoc
                },
                {
                    id: 'accessibility',
                    label: 'Accessibility',
                    component: AccessibilityDoc
                }
            ],
            ptComponent: PTComponent
        };
    }
};
</script>
