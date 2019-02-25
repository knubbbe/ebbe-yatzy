<div class="counter">
    <button class="counter__number" on:click="set({ count: count + 1 })">
        <span>{count}</span>
    </button>
    <button class="counter__reset" on:click="set({ count: 0 })">reset</button>
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
    border: 1px solid #eee;
    border-radius: 100%;
    box-shadow: 2px 2px 15px 0 rgba(0, 0, 0, .1);
    cursor: pointer;
    transition: all .1s ease-in;
}

.counter__number span {
    line-height: 1;
    transition: all .1s ease-in;
}

.counter__number:active {
    box-shadow: 0px 0px 3px rgba(0, 0, 0, .1);
}
.counter__number:active span {
    transform: scale(0.8);
}

.counter__reset {
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
