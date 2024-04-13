<script setup>
import TestimonialsCard from './TestimonialsCard.vue'
import imgwhite from '/src/assets/white.png'
import imgishan from '/src/assets/ishan.png'
import imgprem from '/src/assets/prem.png'
import imgigor from '/src/assets/igor.png'
</script>

<template>

  <div class="testimonials-wrapper">
    <h1>See what people have to say</h1>
     <div class="testimonials-cards-wrapper">
      <TestimonialsCard
        testimonialText="“Laurentino is a beast! Not only does he have great taste, but his product sense, speed of execution, and witty humor make him a joy to work with.”"
        :imageSrc="imgishan"
        name="Ishan Jadhwani"
        position="Founder @ Intellectual Point"
        class="testimonial-card"
      />
      <TestimonialsCard
        testimonialText="“Laurentino is probably the best designer I've ever worked with. Even working with us just 10 hours per week, the quality of his output is better than that of many full-time product designers, making his impact on our team truly remarkable.”"
        :imageSrc="imgwhite"
        name="Cameron Mema"
        position="Founder @ Cyfr Inc."
        class="testimonial-card"
      />
      <TestimonialsCard
        testimonialText="“Laurentino's designs are top tier and he possesses the unique ability to quickly understand product direction, then identify the highest leverage areas for product improvement. Indexing on work with past designers, I'd estimate we saved 10s if not 100s of hours per sprint having Zeuz in the mix.”"
        :imageSrc="imgwhite"
        name="Lorem Ipsum"
        position="Founder @ None"
        class="testimonial-card"
      />
      <TestimonialsCard
        testimonialText="“Laurentino's design genius shines through his ability to deeply internalize an organization's objectives and constraints.  His remarkable ability to synthesize data, consumer insights, and outside-the-box thinking allows him to create truly original work. We couldn't be happier with the results.”"
        :imageSrc="imgprem"
        name="Prem Jadhwani"
        position="Founder @ Neuroscale"
        class="testimonial-card"
      />
      <TestimonialsCard
        testimonialText="“Laurentino is a phenomenal product designer. Since he's been on board, we've gotten immeasurable amounts of positive comments on our website and game design – the transformation has been remarkable. Because of his vast experience working with early-stage companies, he is able to make product & design recommendations that not only streamline development but also resonate with our target market. He's been a cheat code for us, and we're blessed to have him in our corner.”"
        :imageSrc="imgigor"
        name="Igor Alonge"
        position="CTO @ fiveX Corporation"
        class="testimonial-card"
      />
      <TestimonialsCard
        testimonialText="“Laurentino has the speed, insights, instincts, and taste to be my go-to collaborator on our most critical product designs. There’s no challenge I’ve found that time with Zeuz doesn’t help solve.”"
        name="John"
        position="Ex-Admin @ RedeFury"
        class="testimonial-card"
        :imageSrc="imgwhite"
      />
    </div>

  </div>
 
</template>

<style scoped>
  h1{
    font-size: 28px;
    text-align: center;
    padding-bottom: 30px;
    color: white;
  }
  .testimonials-wrapper{
    padding-top: 100px;
    max-width: fit-content;
    width: 100%;
    margin-inline: auto;
    padding-inline: 20px;
  }
  .testimonials-cards-wrapper{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 30px;
  }

  @media (max-width: 1200px) {
    .testimonials-cards-wrapper{
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 30px;
  }
}
  @media (max-width: 768px) {
    .testimonials-cards-wrapper{
    display: grid;
    grid-template-columns: 1fr;
    gap: 30px;
    }
  }
</style>