<script></script>

<button class="primarybutton"> <slot /> </button>

<style>
  .primarybutton {
    border: 1px solid transparent;
    -webkit-transition: all 0.4s cubic-bezier(0.5, 0.24, 0, 1);
    transition: all 0.4s cubic-bezier(0.5, 0.24, 0, 1);
  }
  .primarybutton::before {
    content: "";
    position: absolute;
    left: 0px;
    bottom: 0px;
    z-index: -1;
    width: 0%;
    height: 1px;
    background: #6098ff;
    box-shadow: inset 0px 0px 0px #6098ff;
    display: block;
    -webkit-transition: all 0.4s cubic-bezier(0.5, 0.24, 0, 1);
    transition: all 0.4s cubic-bezier(0.5, 0.24, 0, 1);
  }

  .primarybutton:hover::before {
    width: 100%;
  }

  .primarybutton::after {
    content: "";
    position: absolute;
    right: 0px;
    top: 0px;
    z-index: -1;
    width: 0%;
    height: 1px;
    background: #6098ff;
    -webkit-transition: all 0.4s cubic-bezier(0.5, 0.24, 0, 1);
    transition: all 0.4s cubic-bezier(0.5, 0.24, 0, 1);
  }
  .primarybutton:hover::after {
    width: 100%;
  }
  .primarybutton:hover {
    border-left: 1px solid #6098ff;
    border-right: 1px solid #6098ff;
  }
</style>
