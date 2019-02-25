<div class="counter">
    <div class="counter__number" on:click="set({ count: count + 1 })">
        <span>{count}</span>
    </div>
    <button on:click="set({ count: 0 })">reset</button>
</div>

<style>
.counter {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.counter__number {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 15rem;
    height: 15rem;
    font-size: 6rem;
    background-color: #fff;
    border: 1px solid #fcfcfc;
    border-radius: 100%;
    box-shadow: 2px 2px 10px rgba(0, 0, 0, .1);
    cursor: pointer;
}
.counter__number span {
    line-height: 1;
}

button {
    margin-top: 2rem;
}
</style>

<script>
export default {
    data() {
        return {
            count: 0
        };
    }
}
</script>
