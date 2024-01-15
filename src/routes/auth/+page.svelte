<script>
	let roll_no = 0;
	let pwd = '';
	const submit_user_details = () => {
		console.log(roll_no, pwd);
	};
</script>

<h1>Let's try to authenticate you!</h1>

<div id="auth_form">
	<form>
		<label>
			Roll No: <input type="number" name="roll_no" bind:value={roll_no} />
		</label>
		<br />
		<label>
			Password: <input type="password" name="pwd" bind:value={pwd} />
		</label>
		<br />
		<input type="submit" on:click={submit_user_details} />
	</form>
</div>

<style>
	h1 {
		text-align: center;
	}
	#auth_form input {
		width: 100%;
	}
</style>
