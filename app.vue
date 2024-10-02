<template>
  <link rel="stylesheet" href="assets/css/style.css">
  <header>
		<nav>
			<div class="logo">
				<a href="">
					<img src="./assets/img/logo/nav-logo.png" alt="Rumah Laundry Logo">
				</a>
			</div>
			<ul class="nav-menu">
				<li>
					<span id=""> User</span>
					<ul class="dropdown-menu">
						<li><a href="">Tentang Kami</a></li>
						<li><a href="">Logout</a></li>
					</ul>
				</li>
			</ul>
		</nav>
		<div id="nav-mini">
			<a href="" class="link-nav">Riwayat Transaksi</a>
			<a href="" class="link-nav">Manage Karyawan</a>
			<a href="" class="link-nav">Daftar Paket</a>
		</div>
	</header>
<div id="main" class="main-content">
		<div class="container">
			<div class="baris">
				<div class="selamat-datang">
					<div class="col-header">
						<p class="judul-sm">Selamat Datang </p>
						<h2 class="judul-md">Dashboard</h2>
					</div>

					<div class="col-header txt-right">
						<a href="" class="btn-lg bg-primary">+ Order Baru</a>
					</div>	
				</div>
			</div>

			<div class="baris">
				<div class="col col-4">
					<div class="card">
						<div class="card-body">
							<div class="card-panel">
								<div class="panel-header">
									<p>Jumlah Karyawan</p>
									<h2>$jml_karyawan </h2>
								</div>
								<div class="panel-icon">
									<img src="./assets/img/team.png" alt="karyawan" height="48">
								</div>
							</div>
						</div>
					</div>
				</div>

				<div class="col col-4">
					<div class="card">
						<div class="card-body">
							<div class="card-panel">
								<div class="panel-header">
									<p>Total Order</p>
									<h2> jmlOrder</h2>
								</div>
								
								<div class="panel-icon">
									<img src="./assets/img/total_order.png" alt="order" height="48">
								</div>
							</div>
						</div>
					</div>
				</div>

				<div class="col col-4">
					<div class="card">
						<div class="card-body">
							<div class="card-panel">
								<div class="panel-header">
									<p>Jumlah Paket Tersedia</p>
									<h2> jmlPaket</h2>
								</div>

								<div class="panel-icon">
									<img src="./assets/img/jumlah_paket.png" alt="paket" height="48">
								</div>
							</div>
							
						</div>
					</div>
				</div>
				<div class="col">
   <div class="card">
      <div class="card-title card-flex">
         <div class="card-col">
            <h2>Order Cuci Komplit</h2>	
         </div>
      </div>

      <div class="card-body">
         <div class="tabel-kontainer">
            <table class="tabel-transaksi">
               <thead>
                  <tr>
                     <th class="sticky">No</th>
                     <th class="sticky">No.Order</th>
                     <th class="sticky">Tgl Order</th>
                     <th class="sticky">Nama Pelanggan</th>
                     <th class="sticky">Jenis Paket</th>
                     <th class="sticky">Waktu Kerja</th>
                     <th class="sticky">Berat (Kg)</th>
                     <th class="sticky">Action</th>
                  </tr>
               </thead>

               <tbody>
                        <tr>
                           <td> $no_ck; </td>
                           <td> $ck['or_ck_number'] </td>
                           <td> $ck['tgl_masuk_ck'] </td>
                           <td> $ck['nama_pel_ck'] </td>
                           <td> $ck['jenis_paket_ck'] </td>
                           <td> $ck['wkt_krj_ck'] </td>
                           <td> $ck['berat_qty_ck'] . ' Kg' </td>
                           <td>
                              <a href="url('detail_order/detail_ck/detail_order_ck.php?or_ck_number=')$ck['or_ck_number']" class="btn btn-detail">Detail</a>

                              <a href="url('daftar_order/hapus_ck.php?or_ck_number=')$ck['or_ck_number']" onclick="return confirm('Yakin akan menghapus?');" class="btn btn-hapus">Hapus</a>
                           </td>
                        </tr>
                        
                        <tr>
                           <td colspan="8" class="txt-center">Data Tidak Tersedia</td>
                        </tr>
               </tbody>
            </table>
         </div>
      </div>
   </div>
</div>
			</div>
      </div>
      </div>

</template>
