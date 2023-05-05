<script>
  import { acak } from "kumpulan-tools";
  // @ts-ignore
  import data from "../data.yml";

  let isi;

  function tampil() {
    isi = acak(data)[0];
  }
  tampil();
</script>

<div
  class="min-h-screen w-full grid font-serif items-center p-5"
  on:click={tampil}
>
  <div>
    <div class="text-center text-lg">{isi}</div>
  </div>
</div>
