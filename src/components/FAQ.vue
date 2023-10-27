<template>
  <div class="border-2 h-auto w-full">
    <h2 class="text-center font-semibold md:text-6xl text-4xl my-10">FAQs</h2>
    <Accordion   class="w-[80%] mx-auto py-5">
      <AccordionTab
        v-for="faq of faqs"
        :header="faq.question"
        toggleable
      
      >
        <p>{{ faq.answer }}</p>
      </AccordionTab>
    </Accordion>
  </div>
</template>
<script>
// import Panel from 'primevue/panel';
import Accordion from "primevue/accordion";
import AccordionTab from "primevue/accordiontab";
export default {
  components: {
    Accordion,
    AccordionTab,
  },
  data() {
    return {
      faqs: [
        {
          question: "What products does Zain Amoire offer?",
          answer:
            "Zain Amoire specializes in a range of modest fashion items, including hijabs, palazzo pants, and veils. We offer diverse styles and designs crafted with the utmost care and quality.",
        },
        {
          question: "How can I place an order?",
          answer:
            "Placing an order is easy! Simply browse our online store, select the items you wish to purchase, add them to your cart, and proceed to checkout. Follow the prompts to enter your shipping details and payment information.",
        },
        {
          question: "What payment methods do you accept?",
          answer:
            "We accept major credit cards, debit cards, and secure payment methods like PayPal for a smooth and secure checkout experience.",
        },
        {
          question: "What is your return policy?",
          answer:
            "We want you to be completely satisfied with your purchase. If you're not happy with your order, you can return it within 30 days of receiving the item. Please refer to our Return Policy for detailed information on the process.",
        },
        {
          question: "How can I contact your customer service?",
          answer:
            "Our customer service team is available to assist you. You can reach us via email at support@zainamoire.com or through our Contact Us page on the website. We aim to respond to all inquiries within 24 hours.",
        },
        {
          question: "Are your products ethically sourced?",
          answer:
            "Yes, at Zain Amoire, we are committed to ethical practices. We source our materials responsibly, ensuring fair treatment of workers and sustainable production methods.",
        },
        {
          question: "Can I change or cancel my order after placing it?",
          answer:
            "We process orders quickly to ensure fast shipping. If you need to make changes, please contact us immediately. While we cannot guarantee modifications, we'll do our best to assist you.",
        },
      ],
    };
  },
};
</script>
