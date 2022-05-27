<script lang="ts">
  import { Feature } from '@components';
  import { access, collaboration, file, security } from '@assets';
</script>

<section class="min-bouding w-full mx-auto | lg:max-w-4xl">
  <h2 class="sr-only">Features</h2>
  <div class="grid gap-24 | lg:grid-cols-2">
    <Feature title="Access your files, anywhere" icon={access}>
      The ability to use a smartphone, tablet, or computer to access your account means your files
      follow you everywhere.
    </Feature>
    <Feature title="Security you can trust" icon={security}>
      2-factor authentication and user-controlled encryption are just a couple of the security
      features we allow to help secure your files.
    </Feature>
    <Feature title="Real-time collaboration" icon={collaboration}>
      Securely share files and folders with friends, family and colleagues for live collaboration.
      No email attachments required.
    </Feature>
    <Feature title="Store any type of file" icon={file}>
      Whether you're sharing holidays photos or work documents, Fylo has you covered allowing for
      all file types to be securely stored and shared.
    </Feature>
  </div>
</section>
