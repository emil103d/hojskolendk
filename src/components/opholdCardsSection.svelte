<script>
  import Card from "./card.svelte";
</script>

<section>
  <div class="flex gap-5">
    <div class="relative">
      <div class="z-10 absolute top-40 -left-3">
        <svg
          width="40"
          height="40"
          viewBox="0 0 73 73"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <g filter="url(#filter0_d_637_5477)">
            <circle
              cx="34.5"
              cy="34.5"
              r="34.5"
              transform="rotate(-180 34.5 34.5)"
              fill="white"
            />
          </g>
          <path d="M39.5 48L25 35L39.5 23" stroke="black" stroke-width="2" />
          <defs>
            <filter
              id="filter0_d_637_5477"
              x="0"
              y="0"
              width="73"
              height="73"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix" />
              <feColorMatrix
                in="SourceAlpha"
                type="matrix"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              />
              <feOffset dx="2" dy="2" />
              <feGaussianBlur stdDeviation="1" />
              <feComposite in2="hardAlpha" operator="out" />
              <feColorMatrix
                type="matrix"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.05 0"
              />
              <feBlend
                mode="normal"
                in2="BackgroundImageFix"
                result="effect1_dropShadow_637_5477"
              />
              <feBlend
                mode="normal"
                in="SourceGraphic"
                in2="effect1_dropShadow_637_5477"
                result="shape"
              />
            </filter>
          </defs>
        </svg>
      </div>
      <Card
        title="MALDIVERNE, SRI LANKA, BALI & GILI ISLANDS"
        image="../src/_images/1.jpg"
      />
    </div>

    <Card
      title="MALDIVERNE, SRI LANKA, BALI & GILI ISLANDS"
      image="../src/_images/2.jpg"
    />

    <Card
      title="MALDIVERNE, SRI LANKA, BALI & GILI ISLANDS"
      image="../src/_images/2.jpg"
    />
    <div class="relative">
      <div class="z-10 absolute top-40 -right-3">
        <svg
          width="40"
          height="40"
          viewBox="0 0 73 73"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <g filter="url(#filter0_d_637_5483)">
            <circle cx="34.5" cy="34.5" r="34.5" fill="white" />
          </g>
          <path d="M27 22L41.5 35L27 47" stroke="black" stroke-width="2" />
          <defs>
            <filter
              id="filter0_d_637_5483"
              x="0"
              y="0"
              width="73"
              height="73"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix" />
              <feColorMatrix
                in="SourceAlpha"
                type="matrix"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                result="hardAlpha"
              />
              <feOffset dx="2" dy="2" />
              <feGaussianBlur stdDeviation="1" />
              <feComposite in2="hardAlpha" operator="out" />
              <feColorMatrix
                type="matrix"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.05 0"
              />
              <feBlend
                mode="normal"
                in2="BackgroundImageFix"
                result="effect1_dropShadow_637_5483"
              />
              <feBlend
                mode="normal"
                in="SourceGraphic"
                in2="effect1_dropShadow_637_5483"
                result="shape"
              />
            </filter></defs
          ></svg
        >
      </div>
      <Card
        title="MALDIVERNE, SRI LANKA, BALI & GILI ISLANDS"
        image="../src/_images/2.jpg"
      />
    </div>
  </div>
  <button class=" mx-auto"><a href="/#">SE ALLE OPHOLD</a></button>
</section>
