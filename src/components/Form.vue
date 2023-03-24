<template>
    <form>
        <fieldset class="input-group--all">
          <legend>Write ZIP code here</legend>
          <div class="mb-3">
            <label for="disabledTextInput" class="form-label">Please add valid number(5 symbols)</label>
            <input type="text" id="disabledTextInput" class="form-control" placeholder="ZIP code">
          </div>

          <a  
            href="/" 
            type="submit" 
            class="btn btn-primary custom-btn"
          >
            Render
          </a>
        </fieldset>
      </form>
</template>

<style scoped>
.input-group--all {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%);
    width: 400px;
    background-color: #fff;
    border: solid black 0.5px;
    border-radius: 6px;
}
</style>
