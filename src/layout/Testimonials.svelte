<script>
  import { Testimonial } from '@components';
  import { profile1, profile2, profile3, quotes } from '@assets';
</script>

<section class="relative">
  <h2 class="sr-only">Testimonials</h2>
  <img class="absolute -top-4 left-2 w-6 | lg:(w-auto -top-9 -left-3)" src={quotes} alt="" />
  <div class="relative z-10 grid gap-6 | lg:(grid-cols-3 gap-9)">
    <Testimonial name="Satish Patel" image={profile1}>
      Fylo has improved our team productivity by an order of magnitude. Since making the switch our
      team has become a well-oiled collaboration machine.
    </Testimonial>
    <Testimonial name="Bruce McKenzie" image={profile2}>
      Fylo has improved our team productivity by an order of magnitude. Since making the switch our
      team has become a well-oiled collaboration machine.
    </Testimonial>
    <Testimonial name="Iva Boyd" image={profile3}>
      Fylo has improved our team productivity by an order of magnitude. Since making the switch our
      team has become a well-oiled collaboration machine.
    </Testimonial>
  </div>
</section>
